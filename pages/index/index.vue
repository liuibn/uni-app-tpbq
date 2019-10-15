<template>
	<view class="takePhoto">
		<view class="imageBox">
			<image class="scopeImage leftTop" src="../../static/scopeTL.png" mode="scaleToFill"></image>
			<image class="scopeImage rightTop" src="../../static/scopeTR.png" mode="scaleToFill"></image>
			<image class="getPhoto" :src="photo" mode="aspectFit"></image>
			<image class="scopeImage leftBottom" src="../../static/scopeBL.png" mode="scaleToFill"></image>
			<image class="scopeImage rightBottom" src="../../static/scopeBR.png" mode="scaleToFill"></image>
		</view>
		<view class="bottom">
			<!-- <image class="tipImage" src="../../static/tip.png" mode="widthFix"></image> -->
			<!-- <text>为保障您的权益，本次申请将采集并核实您的身份证信息，请拍摄身份证人像面。</text> -->
			<view class="btnBox">
				<image class="btn1 back" src="../../static/back.png" mode="widthFix"></image>
				<image class="btn1 photoAlbum" src="../../static/photoLibrary.png" mode="widthFix"></image>
				<image class="take" src="../../static/takephoto1.png" mode="widthFix"></image>
				<image class="btn1 submit" src="../../static/submit.png" mode="widthFix"></image>
			</view>
			
		</view>
	</view>
	
</template>


<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.takePhoto{
		display: flex;
		flex-direction: column;
		width: 100%;
		height: 100%;
	}
   .imageBox{
	   display: flex;
	   background-color: #929292;
	   height: 100%;
   }
	   
   .scopeImage{
	   width:  44upx;
	   height: 44upx;
	   
   }
   
   .getPhoto{
	   margin: 90upx 90upx;
	   height: 100%;
	   width: 100%;
   }
	   
   .leftTop{
	  position: absolute;
	   top: 30upx;
	   left: 30upx;
	   
   }
   
   .rightTop{
	   position: absolute;
	   top: 30upx;
	   right: 30upx;
   }
   
   .leftBottom{
   	   position: absolute;
   	   bottom: 30upx;
   	   left: 30upx;
   }
   
   .rightBottom{
   	   position: absolute;
   	   bottom: 30upx;
   	   right: 30upx;
   }
   .bottom{
	   background-color: #000000;
	   width: 100%;
	   height: 200upx;
	   position: fixed;
	   bottom: 0upx;
	   display: flex;
   }
   .tipImage{
	   width: 24upx;
	   height: 24upx;
	   margin-left: 30upx;
	   margin-top: 30upx;
	   
   }
   text{
	   font-size: 24upx;
	   line-height: 10upx;
	   margin: 30upx 30px 30upx 200upx;
   }
   .btnBox{
	   display: flex;
	   flex-direction: row;
       align-items: center;	  
	   justify-content: space-around;
	   width: 100%;
   }
   
   .btn1{
	   width: 60upx;
	   height: 60upx;
   }
   
   .take{
	   width: 80upx;
	   height: 80upx;
   }
   
</style>
