<script lang="ts">
    import ImageCard from '$lib/components/ImageCard.svelte';

    let property = {
        imageUrl: "https://upload.wikimedia.org/wikipedia/commons/d/d0/Aerial_view_of_the_Amazon_Rainforest.jpg",
        imageAlt: "An image of a green forest",
        beds: 3,
        baths: 2,
        title: "A home in a green forest",
        priceInCents: 190000,
        formattedPrice: "$1,900.00",
        reviewCount: 34,
        rating: 4.2
    }


</script>

<h1 class="text-blue-500">This is an image card</h1>

<div class="h-screen flex items-center justify-center bg-gray-200">
    <ImageCard {property}/>
</div>
