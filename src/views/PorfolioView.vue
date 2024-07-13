<script setup>
	import { FwbCarousel } from "flowbite-vue";

	const ecommercePictures = [
		{ src: "images/ecommerce/home.png", alt: "Image 1" },
		{ src: "images/ecommerce/home-search.png", alt: "Image 2" },
		{ src: "images/ecommerce/product.png", alt: "Image 3" },
		{ src: "images/ecommerce/cart.png", alt: "Image 4" },
		{ src: "images/ecommerce/product-crud.png", alt: "Image 5" },
		{ src: "images/ecommerce/user-modal.png", alt: "Image 6" },
	];

	const ecommerceJavaPictures = [
		{ src: "images/ecommerce-java/1_login.png", alt: "Image 1" },
		{ src: "images/ecommerce-java/2_general.png", alt: "Image 2" },
		{ src: "images/ecommerce-java/3_perfil.png", alt: "Image 3" },
		{ src: "images/ecommerce-java/4_usuarios.png", alt: "Image 4" },
		{ src: "images/ecommerce-java/5_usuarios_form.png", alt: "Image 5" },
		{
			src: "images/ecommerce-java/6_usuarios_form_update.png",
			alt: "Image 6",
		},
		{ src: "images/ecommerce-java/7_productos.png", alt: "Image 7" },
		{ src: "images/ecommerce-java/8_pedidos.png", alt: "Image 8" },
		{
			src: "images/ecommerce-java/9_pedidos_historial.png",
			alt: "Image 9",
		},
		{ src: "images/ecommerce-java/10_mesas.png", alt: "Image 10" },
	];
</script>

<template>
	<div class="w-5/6 sm:max-w-6xl mx-auto space-y-10 py-4">
		<div class="space-y-2">
			<h2 class="max-w-3xl mx-auto">Ecommerce básico hecho con laravel 9 y vue 3</h2>
			<fwb-carousel no-indicators :pictures="ecommercePictures" slide class="max-w-3xl h-[200px] sm:h-[300px] md:h-[400px] mx-auto container-carousel z-0" />
		</div>

		<div class="space-y-2">
			<h2 class="max-w-3xl mx-auto">Gestión de un ecommerce hecho con java 17 (proyecto del Sena)</h2>
			<fwb-carousel no-indicators :pictures="ecommerceJavaPictures" slide class="max-w-3xl h-[200px] sm:h-[300px] md:h-[400px] mx-auto container-carousel z-0" />
		</div>
	</div>
</template>

<style>
.container-carousel > div {
	height: 100% !important;
}
.container-carousel > div > div > img {
	height: 100% !important;
	object-fit: contain;
	object-position: top;
}
.container-carousel > button > span {
	background: #222222d7;
}
.container-carousel > button:hover span {
	background: #000000d7 !important;
}
</style>