<template>
<div>
  <h1>Testing imgix video</h1>
  <ul class="flex flex-wrap m-4">
    <li class="xs:w-full md:w-1/2 sm:w-1/2 lg:w-1/3 px-2 xs:mb-6 md:mb-12 article-card">
      <NuxtLink :to="`/video1`" class="flex transition-shadow duration-150 ease-in-out shadow-sm hover:shadow-md flex-col">
        <img src="https://tom.imgix.net/imgix-demo.png?w=400&h=200&fit=crop&crop=faces,edges&auto=format,compress&mark-w=75&mark-align=middle,center&mark=https://tomgcs.imgix.net/playbutton.png?auto=format" />
      <div class="p-6 flex flex-col justify-between w-full">
        <h2 class="font-bold">imgix Demo</h2>
      </div>
      </NuxtLink>
    </li>
    <li class="xs:w-full md:w-1/2 sm:w-1/2 lg:w-1/3 px-2 xs:mb-6 md:mb-12 article-card">
      <NuxtLink :to="`/video2`" class="flex transition-shadow duration-150 ease-in-out shadow-sm hover:shadow-md flex-col">
        <img src="https://tom.imgix.net/legacypinata.png?w=400&h=200&fit=crop&crop=faces,edges&auto=format,compress&mark-w=75&mark-align=middle,center&mark=https://tomgcs.imgix.net/playbutton.png?auto=format" />
      <div class="p-6 flex flex-col justify-between w-full">
        <h2 class="font-bold">Legacy Pinata</h2>
      </div>
      </NuxtLink>
    </li>
    <li class="xs:w-full md:w-1/2 sm:w-1/2 lg:w-1/3 px-2 xs:mb-6 md:mb-12 article-card">
      <NuxtLink :to="`/video3`" class="flex transition-shadow duration-150 ease-in-out shadow-sm hover:shadow-md flex-col">
        <img src="https://tom.imgix.net/izzy_pinata.png?w=400&h=200&fit=crop&crop=faces,edges&auto=format,compress&mark-w=75&mark-align=middle,center&mark=https://tomgcs.imgix.net/playbutton.png?auto=format" />
      <div class="p-6 flex flex-col justify-between w-full">
        <h2 class="font-bold">Izzy Pinata</h2>
      </div>
      </NuxtLink>
    </li>
    <li class="xs:w-full md:w-1/2 sm:w-1/2 lg:w-1/3 px-2 xs:mb-6 md:mb-12 article-card">
      <NuxtLink :to="`/video4`" class="flex transition-shadow duration-150 ease-in-out shadow-sm hover:shadow-md flex-col">
        <img src="https://tom.imgix.net/izzy_dance_party.png?w=400&h=200&fit=crop&crop=faces,edges&auto=format,compress&mark-w=75&mark-align=middle,center&mark=https://tomgcs.imgix.net/playbutton.png?auto=format" />
      <div class="p-6 flex flex-col justify-between w-full">
        <h2 class="font-bold">Izzy Dance Party</h2>
      </div>
      </NuxtLink>
    </li>
    <li class="xs:w-full md:w-1/2 sm:w-1/2 lg:w-1/3 px-2 xs:mb-6 md:mb-12 article-card">
      <NuxtLink :to="`/video5`" class="flex transition-shadow duration-150 ease-in-out shadow-sm hover:shadow-md flex-col">
        <img src="https://tom.imgix.net/image_opt.png?w=400&h=200&fit=crop&crop=faces,edges&auto=format,compress&mark-w=75&mark-align=middle,center&mark=https://tomgcs.imgix.net/playbutton.png?auto=format" />
      <div class="p-6 flex flex-col justify-between w-full">
        <h2 class="font-bold">Image Optimization</h2>
      </div>
      </NuxtLink>
    </li>
    <li class="xs:w-full md:w-1/2 sm:w-1/2 lg:w-1/3 px-2 xs:mb-6 md:mb-12 article-card">
      <NuxtLink :to="`/video6`" class="flex transition-shadow duration-150 ease-in-out shadow-sm hover:shadow-md flex-col">
        <img src="https://tom.imgix.net/zeekava01.png?w=400&h=200&fit=crop&crop=faces,edges&auto=format,compress&mark-w=75&mark-align=middle,center&mark=https://tomgcs.imgix.net/playbutton.png?auto=format" />
      <div class="p-6 flex flex-col justify-between w-full">
        <h2 class="font-bold">Zeek & Eva Running</h2>
      </div>
      </NuxtLink>
    </li>
    <li class="xs:w-full md:w-1/2 sm:w-1/2 lg:w-1/3 px-2 xs:mb-6 md:mb-12 article-card">
      <NuxtLink :to="`/video7`" class="flex transition-shadow duration-150 ease-in-out shadow-sm hover:shadow-md flex-col">
        <img src="https://tom.imgix.net/cantilever_imgix_lowq_test.png?w=400&h=200&fit=crop&crop=faces,edges&auto=format,compress&mark-w=75&mark-align=middle,center&mark=https://tomgcs.imgix.net/playbutton.png?auto=format" />
      <div class="p-6 flex flex-col justify-between w-full">
        <h2 class="font-bold">imgix Cantilever Promo</h2>
      </div>
      </NuxtLink>
    </li>
    <li class="xs:w-full md:w-1/2 sm:w-1/2 lg:w-1/3 px-2 xs:mb-6 md:mb-12 article-card">
      <NuxtLink :to="`/video8`" class="flex transition-shadow duration-150 ease-in-out shadow-sm hover:shadow-md flex-col">
        <img src="https://tom.imgix.net/gender_reveal.jpg?w=400&h=200&fit=crop&crop=faces,edges&auto=format,compress&mark-w=75&mark-align=middle,center&mark=https://tomgcs.imgix.net/playbutton.png?auto=format" />
      <div class="p-6 flex flex-col justify-between w-full">
        <h2 class="font-bold">Gender Reveal Race</h2>
      </div>
      </NuxtLink>
    </li>
    <li class="xs:w-full md:w-1/2 sm:w-1/2 lg:w-1/3 px-2 xs:mb-6 md:mb-12 article-card">
      <NuxtLink :to="`/video9`" class="flex transition-shadow duration-150 ease-in-out shadow-sm hover:shadow-md flex-col">
        <img src="https://tom.imgix.net/grandma_dance.png?w=400&h=200&fit=crop&crop=faces,edges&auto=format,compress&mark-w=75&mark-align=middle,center&mark=https://tomgcs.imgix.net/playbutton.png?auto=format" />
      <div class="p-6 flex flex-col justify-between w-full">
        <h2 class="font-bold">Grandma Dance</h2>
      </div>
      </NuxtLink>
    </li>
  </ul>
</div>
</template>

<script>
export default {
  /*data: () => ({
    videos: [
      { id: 0, title:'imgix Demo Video', hls:'https://tomgcs.imgix.cc/imgix-demo.mov?fm=hls'},
      { id: 1, title:'Legacy Pinata', hls:'https://tomgcs.imgix.cc/legacypinata.mov?fm=hls'},
      { id: 2, title:'Izzy Pinata', hls:'https://tom.imgix.net/zeek_tmnt.jpg?w=400&auto=format,compress'}
    ]
  })*/
}
</script>
<style>
.player {
  width: 400px;
  margin: 0 auto;
  min-height: 30px;
}
</style>
