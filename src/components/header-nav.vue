<template>
	<div id="header">
		<div class="nav-global">
			<div class="container">
				<h1 class="nav-logo">
					<a href="javascript:;"></a>
				</h1>
				<ul class="nav-aside">
					<li class="nav-user">
					  <router-link to="/account">个人中心</router-link>
						<!--active-->
						<div class="nav-user-wrapper">
							<div class="nav-user-list">
								<dl class="nav-user-avatar">
									<dd><span class="ng-scope"></span></dd>
									<dt class="ng-binding">+86 158****990</dt>
								</dl>
								<ul>
									<li class="order"><router-link to="/account" exact>我的订单</router-link></li>
									<!--<li class="support"><a href="javascript:;">售后服务</a></li>
									<li class="coupon"><a href="javascript:;">我的优惠</a></li>
									<li class="information"><a href="javascript:;">账户资料</a></li>-->
									<li class="address"><router-link to="/address">收货地址</router-link></li>
								<!--	<li class="logout"><a href="javascript:;">退出</a></li>-->
								</ul>
							</div>
						</div>
					</li>
					<!--active-->
					<car-panel class="nav-cart"></car-panel>
				</ul>
				<ul class="nav-list">
					<li><a href="javascript:;">首页</a></li>
					<li><a href="javascript:;">书城</a></li>
					<li><a href="javascript:;">售后服务</a></li>
					<li><a href="javascript:;">联系我们</a></li>
				</ul>
			</div>
		</div>
		<div class="nav-sub">
			<div class="nav-sub-wrapper">
				<div class="container">
					<ul class="nav-list">
						<li><a href="javascript:;">书们</a></li>
						<router-link to="/" exact tag="li" activeClass="active">
						    <a>最新书们</a>
						</router-link>
						<li><a href="javascript:;">为你推荐</a></li>
					</ul>
				</div>
			</div>
		</div>
	</div>
</template>
<script>
import CarPanel from '@/components/car-panel'
export default {
  components: {
    CarPanel
  }
}
</script>
