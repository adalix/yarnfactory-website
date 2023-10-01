<template>
    <Navbar/>
    <div class="flex flex-col">
        <div class="flex justify-between w-4/5 mx-auto bg-orange-300">
			<h1 class="font-medium text-2xl">TUM URUNLER</h1>
            <select name="" id="" class="border-2 border-solid p-2 focus:ouline-none">
                <option>Tumu</option>
                <option>Yunler</option>
                <option>Tiglar</option>
                <option>Modeller</option>
                <option>sort by sale</option>
            </select>
		</div>
        <div class="mt-2 h-full w-4/5 mx-auto">
            <div class="grid grid-cols-1 gap-4 place-items-center sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-5 lg:w-full ">
                <!-- CARD -->
                <div class="w-[250px] h-[350px] backdrop-blur-xl bg-white/30 shadow-lg rounded-md ">
                    <div class="card-image">
                        <img class="w-[250px] h-[270px] mx-auto rounded-t-lg" src="/nako-calico-bebe.png" alt=""/>
                    </div>
                    <div class="card-content pt-2 px-3">
                        <div class="text-gray-900 text-xl font-bold pb-2">
                            <h2>Nako <span>Callico</span></h2>
                        </div>
                        <div class="text-gray-900">
                            <span class="mr-5">Renk kodu: 70451</span>
                            <span>Stok: 9</span>
                        </div>
                    </div>
                </div>
                <!-- CARD -->
                <div class="w-[250px] h-[350px] backdrop-blur-xl bg-white/30 shadow-lg rounded-md">
                    <div class="card-image">
                        <img class="w-[250px] h-[270px] mx-auto rounded-t-lg" src="/sis.png" alt="" />
                    </div>
                    <div class="card-content pt-2 px-3">
                        <div class="text-gray-900 text-xl font-bold pb-2">
                            <h2>Nako</h2>
                        </div>
                        <div class="text-gray-900">
                            <span class="mr-5"><span>Tig</span> No:1</span>
                            <span>Stok: 1</span>
                        </div>
                    </div>
                </div>
                <!-- CARD -->
            </div>
        </div>
    </div>
</template>

<script>
import Navbar from './Navbar.vue';
export default {
    components:{Navbar},
    setup () {
        

        return {Navbar}
    }
}
</script>
