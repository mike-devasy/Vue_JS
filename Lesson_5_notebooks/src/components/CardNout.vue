<template>
	<div class="container">
<div class="image">
	<img :src="noutData.imgSrc" alt="nout">
</div>
<div class="content">
	<h1 class="title">{{noutData.title}}</h1>
	<p class="discount-price">Ваша економія <span>{{noutData.discount}}₴</span></p>
	<p class="old-price">{{noutData.oldPrice}}₴</p>
<div class="price-line">
	<span class="price">{{noutData.price}}₴</span>
	<button>Купити</button>
</div>
</div>

	</div>
</template>

<script>
	export default {
		name:'CardNout',
		props: {
			noutData: {
				type: Object,
				default: ()=>({})
			},
		},
	}
</script>

<style lang="css" scoped>
.container{
width: 700px;
display: flex;
justify-content: space-between;
/* flex-wrap: wrap; */
}
.image{
	padding-top: 15px;
	width: 200px;
height: 200px;
}
.image img{
width: 100%;
} 
.content{
padding-left: 15px;
}
.title{
font-size: 25px;
}
.discount-price {
text-align: left;
}
.discount-price span, .price{
	color: red;
}
.old-price{
text-align: left;
text-decoration: line-through;
}

.price-line {
display: flex;
justify-content: space-between;
text-align: left;
}
button{
width: 90px;
background-color: rgb(22, 179, 48);
color: whitesmoke;
border:none;
border-radius:5px;
}
.price {
font-size: 28px;
font-weight: 500;
}

</style>