
<script>

    import StarSvg from './StarSVG.svelte';

    export let property = {
        imageUrl: "https://upload.wikimedia.org/wikipedia/commons/d/d0/Aerial_view_of_the_Amazon_Rainforest.jpg",
        imageAlt: "An image of a forest",
        beds: 3,
        baths: 2,
        title: "A home in a forest",
        priceInCents: 190000,
        formattedPrice: "$1,900.00",
        reviewCount: 34,
        rating: 4 
    }

</script>


<div class="">
    <div class="bg-white border rounded-lg overflow-hidden max-w-md">
        <img src="{property.imageUrl}" alt={property.imageAlt}>
        <div class="p-6">
            <div class="flex items-baseline">
                <span class="inline-block bg-teal-100 text-teal-800 text-xs px-2 rounded-lg uppercase font-semibold tracking-wide">New</span>

                <div class="ml-2 text-gray-600 text-xs font-semibold uppercase tracking-wide">{property.beds} beds &bull; {property.baths} baths</div>
            </div>
            <h4 class="mt-1 font-semibold text-lg leading-snug truncate">{property.title}</h4>
            <div class="mt-1">
                {property.formattedPrice} <span class="text-gray-600 text-sm">/ week</span>
            </div>
            
            <div class="mt-4 flex items-center">
                <StarSvg rating={property.rating}/> <span class="text-gray-600 text-sm ml-2">{property.reviewCount} reviews</span>
            </div>
        </div>
    </div>
</div>