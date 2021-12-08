<template>
    <div>
        <div class="min-h-screen bg-gray-100">
            <!-- Navbar goes here -->
	<nav class="bg-white shadow-lg">
		<div class="max-w-6xl mx-auto px-4">
			<div class="flex justify-between">
				<div class="flex space-x-7">
					<!-- Website Logo -->
					<div class="flex items-center py-4 px-2" >
					
                            <Link >
							<BreezeApplicationLogo alt="Logo" class="h-8 w-8 mr-2" />
							<span class="font-semibold text-gray-500 text-lg"
								>Navigation</span
							>
						</Link>
					</div>
				
				</div>
			</div>
		</div>
	</nav>

    <main>
        <slot />
    </main>

        </div>
    </div>
</template>

<script>
import BreezeApplicationLogo from '@/Components/ApplicationLogo.vue';
import { Link } from '@inertiajs/inertia-vue3';
export default {
    components: {
        BreezeApplicationLogo,
        Link,
    },

    setup() {
        
    },
}
</script>