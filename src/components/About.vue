<template>
	<div>
		<h2><strong>Bootstrap 大礼包</strong></h2>
		<table class="table table-bordered table-striped">
			<thead>
				<tr>
					<th class="text-center">作用</th>
					<th class="text-center">标签/类名</th>
					<th class="text-center">效果</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<td>删除符</td>
					<td>&lt;del&gt;删除的文字&lt;/del&gt;</td>
					<td><del>删除的文字</del></td>
				</tr>
				<tr>
					<td>下划线</td>
					<td>&lt;u&gt;下划线&lt;/u&gt;</td>
					<td><u>下划线</u></td>
				</tr>
				<tr>
					<td>文字居中</td>
					<td>&lt;div class="text-center"&gt;文字位置&lt;/div&gt;可选项：'text-left' 'text-right'</td>
					<td><div class="text-center">文字居中</div></td>
				</tr>
				<tr>
					<td>改变大小写</td>
					<td>&lt;del&gt;words&lt;/del&gt;可选项：'text-lowercase' 'text-capitalize'</td>
					<td><div class="text-uppercase">words</div></td>
				</tr>
				<tr>
					<td>基本缩略语</td>
					<td>&lt;del&gt;HTML&lt;/del&gt;</td>
					<td><abbr title="HyperText Markup Language">HTML</abbr></td>
				</tr>
				<tr>
					<td>引用样式</td>
					<td>&lt;blockquote class="blockquote-reverse"&gt;引用样式&lt;/blockquote&gt;</td>
					<td>
					<blockquote class="blockquote-reverse">
					  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
					  <footer>Someone famous in <cite title="Source Title">Source Title</cite></footer>
					</blockquote></td>
				</tr>
			</tbody>
		</table>
	</div>
</template>

<script type="text/javascript">
	export default {
		name: 'About'
	}
</script>