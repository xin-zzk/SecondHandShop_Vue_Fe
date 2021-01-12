<template>
	<view class="container">
		<view class="show_contain">
			<view class="left_contain">
				<view class="item_contain" 
				v-for="(item,index) in leftList">
				<view class="item_show">
					<image class="item_img" src="http://www.suwenzhao.xyz/dog.jpg"></image>
				{{item}}
				</view>
				</view>
			</view>
			<view class="right_contain">
				<view class="item_contain" 
				v-for="(item,index) in rightList">
				<view class="item_show">
					<image class="item_img" src="http://www.suwenzhao.xyz/dog.jpg"></image>
					{{item}}
				</view>
				</view>
			</view>
		</view>
		
		<!-- <text class="intro">详见：</text>
		<uni-link :href="href" :text="href"></uni-link> -->
	</view>
</template>

<style>
	.container {
		height:auto;
		width:340px;
		display: flex;
		/* padding:0,20px; */
	}
	.show_contain{
		height:auto;
		width:auto;
		display: flex;
	}
	.left_contain{
		height: auto;
		width: 48%;
		padding: 0 1%;
	/* 	float:left; */
		/* flex-direction:row-reverse; */
		flex-wrap:wrap ;
	}
	.right_contain{
		height: auto;
		width: 45%;
		padding: 0 1%;
	/* 	float: left; */
	/* 	flex-direction:row-reverse; */
		flex-wrap:wrap ;
	}
	.item_contain{
	/* 	height:100px;
		width:100px; */
		width:160px;
		height:110px;
		float:left;
		display:flex;
		padding-bottom: 50rpx;
	}
	.item_show{
		height:auto;
		/* width: 100px; */
		width:45%;
		border: 1px solid black;
		position:fixed;
	}
	.item_img{
		width:160px;
		height:102px;
	}
	
</style>


<script>
	export default {
		data() {
			return {
				leftList:["1","2"],
				rightList:["3","4"],
				href: 'https://uniapp.dcloud.io/component/README?id=uniui'
			}
		},
		methods: {

		}
	}
</script>


