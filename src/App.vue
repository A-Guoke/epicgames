<template>
        <!-- 头部 -->
        <header>
      <!-- 顶部导航条 -->
      <div id="top-nav">
        <div class="nav">
          <i class="iconfont icon-epicgames"></i>
          <!-- 菜单图标 -->
          <div class="menu-icon">
            <div class="menu-icon-lines"></div>
            <div class="menu-icon-lines"></div>
            <div class="menu-icon-lines"></div>
          </div>
        </div>
        <!-- 菜单 -->
        <div class="menu">
          <!-- 导航 -->
          <ul>
            <li>
              <a href="#" class="text-55px">商城</a>
            </li>
            <li>
              <a href="#">常见问题</a>
            </li>
            <li>
              <a href="#">帮助</a>
            </li>
            <li>
              <a href="#">虚幻引擎</a>
            </li>
          </ul>
          <!-- 登录、切换语言、获取客户端的盒子 -->
          <div class="menu-right">
            <div class="login-box">
              <a href="#">
                <i class="iconfont icon-user"></i>
                <span> 登录 </span>
              </a>
            </div>
            <div class="local-box">
              <a href="#">
                <i class="iconfont icon-earth"></i>
              </a>
            </div>
            <div class="get-client">
              <a href="#">获取客户端 </a>
            </div>
          </div>
        </div>
      </div>
    </header>
    <!-- 主要内容 -->
    <main>
      <div id="container">
        <!-- 搜索和切换分类 -->
        <div id="search-category-box">
          <!-- 搜索框 -->
          <div class="search-box">
            <i class="iconfont icon-search"></i>
            <input type="text" placeholder="搜索" />
            <i class="iconfont icon-close"></i>
          </div>
          <!-- 切换分类 -->
          <div class="toggle-category">
            <div>探索</div>
          </div>
          <div class="space"></div>
        </div>
        <!-- 轮播图 -->
        <div id="rotating-image">
          <!-- 轮播的图片 -->
          <div class="rotating-img-group">
            <a href="#1" style="z-index: 1">
              <picture>
                <source
                  media="(min-width: 768px)"
                  srcset="@/assets/img/1920x1080.jpg"
                />
                <img src="@/assets/img/640x854.jpg" />
              </picture>
            </a>
            <a href="#2">
              <picture>
                <source
                  media="(min-width: 768px)"
                  srcset="@/assets/img/1920x1080.jpg"
                />
                <img src="@/assets/img/640x854.jpg" />
              </picture>
            </a>
            <a href="#3">
              <picture>
                <source
                  media="(min-width: 768px)"
                  srcset="@/assets/img/1920x1080.jpg"
                />
                <img src="@/assets/img/640x854.jpg" />
              </picture>
            </a>
          </div>
          <!-- 轮播的切换按钮 -->
          <div class="rotating-toggle-btn-group">
            <div class="r-active">
              <div class="rotating-toggle-point"></div>
              <div class="rotating-toggle-btn-describe">
                <div>
                  <img src="@/assets/img/640x854.jpg" alt="" />
                  <span>《red》</span>
                </div>
              </div>
            </div>
            <div>
              <div class="rotating-toggle-point"></div>
              <div class="rotating-toggle-btn-describe">
                <div>
                  <img src="@/assets/img/640x854.jpg" alt="" />
                  <span>《blue》</span>
                </div>
              </div>
            </div>
            <div>
              <div class="rotating-toggle-point"></div>
              <div class="rotating-toggle-btn-describe">
                <div>
                  <img src="@/assets/img/640x854.jpg" alt="" />
                  <span>《green》</span>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- 特惠游戏 -->
        <div id="discount-games">
          <h2>特惠游戏</h2>
          <div class="card-list">
            <!-- 一个竖着的卡片 -->
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <!--  -->
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
          </div>
        </div>
        <!-- 最近发售 -->
        <div id="new-release">
          <h2>最近发售</h2>
          <div class="card-list">
            <!-- 一个竖着的卡片 -->
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-price">$8.88</div>
              </div>
            </div>
            <!--  -->
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
          </div>
        </div>
        <!-- 推荐游戏 -->
        <div id="recommend-game">
          <img src="@/assets/img/1920x1080.jpg" alt="" />
          <div class="card">
            <div class="card-title">《title title》- 立省100%</div>
            <div class="card-describe">
              This is a description! This is a description! 立省100%!
            </div>
            <div class="card-about-price">
              <div class="card-discount">-0%</div>
              <div class="card-original-price">$8.88</div>
              <div class="card-price-after-discount">$8.88</div>
            </div>
            <div class="more-btn">
              <a href="#" class="card-btn-link">
                <el-button class="card-btn">立享优惠!</el-button>
              </a>
              <button class="add-wishlist">
                <i class="iconfont icon-plus-circle"></i>
                <span>添至愿望清单!</span>
              </button>
            </div>
          </div>
        </div>
        <!-- 免费游戏 -->
        <div id="free-games">
          <div class="title-box">
            <div class="title">
              <i class="iconfont icon-gift"></i>
              <h2>免费游戏</h2>
            </div>
            <button class="see-more-btn">查看更多</button>
          </div>

          <div class="free-games-card-list">
            <div class="lcard">
              <div class="lcard-img-box">
                <img src="@/assets/img/1920x1080.jpg" alt="" />
                <div class="lcard-img-bottom-banner now">现在免费</div>
              </div>
              <div class="lcard-title">title-title</div>
              <div class="lcard-describe">当前免费, 2月25日00:00截止</div>
            </div>

            <div class="lcard">
              <div class="lcard-img-box">
                <img src="@/assets/img/1920x1080.jpg" alt="" />
                <div class="lcard-img-bottom-banner">即将推出</div>
              </div>
              <div class="lcard-title">title - title</div>
              <div class="lcard-describe">免费 2月25日 - 3月04日</div>
            </div>
          </div>
        </div>
        <!-- 排行榜 -->
        <div id="rank-lists">
          <!-- 三个排行榜 -->
          <ul>
            <li>
              <div class="title-box">
                <div class="title">全新发行</div>
                <button class="see-more-btn">查看更多</button>
              </div>
              <ul>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
              </ul>
            </li>
            <li>
              <div class="title-box">
                <div class="title">最畅销</div>
                <button class="see-more-btn">查看更多</button>
              </div>
              <ul>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
              </ul>
            </li>
            <li>
              <div class="title-box">
                <div class="title">即将推出</div>
                <button class="see-more-btn">查看更多</button>
              </div>
              <ul>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
                <li>
                  <div class="rcard">
                    <div class="img-box">
                      <img src="@/assets/img/640x854.jpg" alt="" />
                    </div>
                    <div class="rcard-text">
                      <div class="rcard-title">title-title</div>
                      <div class="rcard-about-price">
                        <div class="rcard-discount">-0%</div>
                        <div class="rcard-original-price">$8.88</div>
                        <div class="rcard-price-after-discount">$8.88</div>
                      </div>
                    </div>
                  </div>
                </li>
              </ul>
            </li>
          </ul>
          <!-- 选择列表按钮 -->
          <div class="switch-list">
            <div class="btn-p">
              <div class="switch-btn active"></div>
            </div>
            <div class="btn-p">
              <div class="switch-btn"></div>
            </div>
            <div class="btn-p">
              <div class="switch-btn"></div>
            </div>
          </div>
        </div>
        <!-- 两个推荐游戏 -->
        <div id="two-recommended-games">
          <div class="recommend-list">
            <div class="lcard">
              <div class="lcard-img-box">
                <img src="@/assets/img/1920x1080.jpg" alt="" />
              </div>
              <div class="lcard-text">
                <div class="lcard-title">title-title</div>
                <div class="lcard-describe">
                  this is a description! this is a description! this is a
                  description! this is a description! this is a description!
                  this is a description! this is a description!
                </div>
                <div class="focus">了解详情</div>
              </div>
            </div>

            <div class="lcard">
              <div class="lcard-img-box">
                <img src="@/assets/img/1920x1080.jpg" alt="" />
              </div>

              <div class="lcard-text">
                <div class="lcard-title">title - title</div>
                <div class="lcard-describe">
                  this is a description! this is a description! this is a
                  description! this is a description! this is a description!
                  this is a description! this is a description!
                </div>
                <div class="focus">$60</div>
              </div>
            </div>
          </div>

          <!-- 选择列表按钮 -->
          <div class="switch-list">
            <div class="btn-p">
              <div class="switch-btn active"></div>
            </div>
            <div class="btn-p">
              <div class="switch-btn"></div>
            </div>
          </div>
        </div>
        <!-- 最近更新 -->
        <div id="recently-updated">
          <h2>最近更新</h2>
          <div class="card-list">
            <!-- 一个竖着的卡片 -->
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <!--  -->
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
          </div>
        </div>
        <!-- 最受欢迎 -->
        <div id="most-popular">
          <h2>最受欢迎</h2>
          <div class="card-list">
            <!-- 一个竖着的卡片 -->
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <!--  -->
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
          </div>
        </div>
        <!-- 游戏商城最新上架 -->
        <div id="new-arrival">
          <h2>游戏商城最新上架</h2>
          <div class="card-list">
            <!-- 一个竖着的卡片 -->
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-price">$8.88</div>
              </div>
            </div>
            <!--  -->
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
            <div class="card">
              <img src="@/assets/img/640x854.jpg" alt="" />
              <div class="card-title">title title</div>
              <div class="card-about-price">
                <div class="card-discount">-0%</div>
                <div class="card-original-price">$8.88</div>
                <div class="card-price-after-discount">$8.88</div>
              </div>
            </div>
          </div>
        </div>
        <!-- 浏览完整目录 -->
        <div id="browse">
          <img src="@/assets/img/1920x1080.jpg" alt="" />
          <div class="card">
            <div class="card-title">浏览完整目录</div>
            <div class="card-describe">
              This is a description! This is a description! 立省100%!
            </div>
            <div class="more-btn">
              <a href="#" class="card-btn-link">
                <button class="card-btn">了解详情</button>
              </a>
            </div>
          </div>
        </div>
      </div>
      <!-- 遮罩覆盖层 -->
      <div class="overlay"></div>
    </main>
    <!-- 页脚 -->
    <footer>
      <!-- 图标 -->
      <div id="icon-list">
        <div class="social">
          <a href="#">
            <i class="iconfont icon-facebook"></i>
          </a>
          <a href="#">
            <i class="iconfont icon-twitter"></i>
          </a>
          <a href="#">
            <i class="iconfont icon-youtube"></i>
          </a>
        </div>
        <div class="scroll-up">
          <a href="#">
            <i class="iconfont icon-up-square"></i>
          </a>
        </div>
      </div>

      <!-- 第一行链接 -->
      <div class="footer-link">
        <div class="link-title">资源</div>
        <div class="link-list-box">
          <ul>
            <li><a href="#">创作者支持计划</a></li>
            <li><a href="#">在Xxxx Xxxx上发布</a></li>
            <li><a href="#">职业</a></li>
            <li><a href="#">公司</a></li>
          </ul>
          <ul>
            <li><a href="#">爱好者作品政策</a></li>
            <li><a href="#">用户体验调查</a></li>
            <li><a href="#">商城最终用户授权协议</a></li>
          </ul>
          <ul>
            <li><a href="#">在线服务</a></li>
            <li><a href="#">社区守则</a></li>
            <li><a href="#">Xxxx Newsroom</a></li>
          </ul>
        </div>
      </div>

      <!-- 第二行链接 -->
      <div class="footer-link">
        <div class="link-title">由Xxxx Xxxx开发</div>
        <div class="link-list-box">
          <ul>
            <li><a href="#">Xxxx Xxxx</a></li>
            <li><a href="#">Xxxx Xxxx</a></li>
            <li><a href="#">Xxxxxxxxx</a></li>
          </ul>
          <ul>
            <li><a href="#">Xxxxxxx Xxxx</a></li>
            <li><a href="#">Xxxxxxxx</a></li>
            <li><a href="#">Xxxx Xxxxxxxx</a></li>
          </ul>
        </div>
      </div>

      <hr />

      <div id="copyright">
        © 2022, Sit consectetur labore nostrud sit incididunt reprehenderit
        laboris occaecat cupidatat enim ea cupidatat reprehenderit occaecat.
        Mollit ad non commodo elit esse in duis sint minim. Voluptate tempor ex
        irure labore aute culpa velit sit commodo tempor Lorem voluptate. Cillum
        anim ea quis minim sit tempor aliqua tempor duis aute. Ut proident
        dolore irure cupidatat proident dolor culpa officia voluptate qui.
      </div>

      <div class="footer-more-link">
        <a href="#">服务条款</a>
        <a href="#">隐私政策</a>
        <a href="#">商店退款政策</a>
      </div>
    </footer>

</template>

<script setup lang="ts">

</script>

<style scoped>
/*下划线跟随*/
ul{
        display: flex;
        position: initial;
    }
    li{
        position: relative;
        padding: 1em 2em;
        font-size: 12px;
        list-style: none;
        white-space:nowrap;
        width: 25%;
        text-align: center;
    }
    li.current_li{
        list-style-type:none;
        border-bottom:2px solid red;
        padding-bottom: 2px;
    }
    a:active, a:hover, a.current {
        color: #ff231c;
    }
    li::after{
        content: '';
        position: absolute;
        bottom: 0;
        width: 0;
        height: 2px;
        color: #ff231c;
        background-color: #ff231c;
        transition: .5s all linear;
    }
    li:hover::after{
        width: 100%;
    }
    li::after{
        left: 100%;     /*选中项上一个下划线收回的方向，从左往右收线*/
    }
    li:hover::after{
        left: 0;      /*选中项下划线出线的方向，从左往右出线*/
    }
    li:hover ~ li::after {
        left: 0;    /*选中项下一个下划线出线的方向，从左往右收线*/
    }
</style>
