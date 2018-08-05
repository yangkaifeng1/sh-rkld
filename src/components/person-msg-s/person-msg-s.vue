<template>
	<div class="person-msg-s">
		<el-row :gutter="10">
			<el-col :span="6">
				<img src="./img/avatar.jpg" class="avatar">
      </el-col>
      <el-col :span="9">
      	<el-row class="key-item">
					<el-col :span="12">姓名：</el-col>
		      <el-col :span="12">忆苦饭</el-col>
		    </el-row>
		    <el-row class="key-item">
					<el-col :span="12">流入时间：</el-col>
		      <el-col :span="12">2018-01-11</el-col>
		    </el-row>
		    <el-row class="key-item">
					<el-col :span="12">标签信息：</el-col>
		      <el-col :span="12">忆苦饭</el-col>
		    </el-row>
      </el-col>
      <el-col :span="9">
      	<el-row class="key-item">
					<el-col :span="12">身份证：</el-col>
		      <el-col :span="12">1111111111111</el-col>
		    </el-row>
		     <el-row class="key-item">
					<el-col :span="12">户籍地址：</el-col>
		      <el-col :span="12">甘肃省秦安先</el-col>
		    </el-row>
		    <el-row class="key-item get-detail">详情</el-row>
      </el-col>
    </el-row>
	</div>
</template>

<script>
	export default {
		name: 'personMsgS'
	}
</script>

<style lang="less" scoped>
	.person-msg-s{
		padding: 5px 0;
		font-size: 12px;
		.avatar{
			background: blue;
			width: 100%;
		}
		.key-item{
			padding: 10px 0;
			&.get-detail{
				color: #409eff; 
				cursor: pointer;
			}
		}
		.el-col{
			text-overflow: ellipsis;
  		overflow: hidden;
 			white-space: nowrap;
		}
		
	}
</style>
