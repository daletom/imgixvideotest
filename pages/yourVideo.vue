<template>
  <div class="player">
    <h3 class="ml-4">Using Nuxt, testing an imgix video with video.js 7 player</h3>
    <h4 class="ml-4">Enter your own HLS video below and press play</h4>
    <br>
    <div class="ml-4">
      <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded" @click="switchPlayer">Play</button> &nbsp;
      <input class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" type="text" v-model="src" style="width: 500px">
    </div>
    <br>
    <client-only>
      <video-player ref="videoPlayer"
                    class="vjs-custom-skin"
                    :options="playerOptions"
                    @play="onPlayerPlay($event)"
                    @ready="onPlayerReady($event)"/>
    </client-only>
  </div>
</template>

<script>
export default {
  name: "index",
  data() {
    return {
      src: 'https://bitdash-a.akamaihd.net/content/sintel/hls/playlist.m3u8',
      playerOptions: {
        autoplay: true,
        controls: true,
        controlBar: {
          timeDivider: false,
          durationDisplay: false
        }
      }
    }
  },
  methods: {
    onPlayerPlay(player) {
    },
    onPlayerReady(player) {
    },
    playVideo: function (source) {
      const player = this.$refs.videoPlayer.player
      const video = {
        withCredentials: false,
        type: 'application/x-mpegurl',
        src: source
      }
      player.reset() // in IE11 (mode IE10) direct usage of src() when <src> is already set, generated errors,
      player.src(video)
      // this.player.load()
      player.play()
    },
    switchPlayer: function () {
      this.playVideo(this.src)
    }
  },
  mounted() {
  }
}
</script>

<style scoped>
.player {
  position: absolute !important;
  width: 100%;
  height: 100%;
}
.vjs-custom-skin {
  height: 90% !important;
}
.vjs-custom-skin /deep/ .video-js {
  width: 100% !important;
  height: 90%;
}
</style>