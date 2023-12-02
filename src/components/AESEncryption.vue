
<!-- AES加密及解密 -->
<template>
      <div>
    <input type="text" v-model="plaintext" placeholder="Username" />
    <input type="password" v-model="jsonStr" placeholder="Password" />
    <button @click="AES_Encrypt">Register</button>
    <button @click="AES_Decrypt">Login</button>
  </div>
</template>

<script lang="ts" setup>
// 使用 bcrypt.js 进行密码加密
import CryptoJS from 'crypto-js'
import { ref } from 'vue';
 
/**
 * AES 加密
 * @param word: 需要加密的文本
 * KEY: // 需要前后端保持一致
 * mode: ECB // 需要前后端保持一致
 * pad: Pkcs7 //前端 Pkcs7 对应 后端 Pkcs5
 */

const plaintext = ref('')
const jsonStr = ref('')

const KEY = CryptoJS.enc.Utf8.parse('d7b85f6e214abcde')
 
const AES_Encrypt = () => {
  let ciphertext = CryptoJS.AES.encrypt(plaintext.value, KEY, {
    mode: CryptoJS.mode.ECB,
    padding: CryptoJS.pad.Pkcs7
  }).toString()
  console.log(ciphertext)
  return ciphertext
}
 
/**
 * AES 解密
 * @param jsonStr
 */
const AES_Decrypt = () => {
  let plaintext = CryptoJS.AES.decrypt(jsonStr.value, KEY, {
    mode: CryptoJS.mode.ECB,
    padding: CryptoJS.pad.Pkcs7
  }).toString(CryptoJS.enc.Utf8)
  console.log(plaintext)

  return plaintext
}
</script>

<style scoped lang="scss">

</style>