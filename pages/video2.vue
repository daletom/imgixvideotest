<template>
  <div class="player">
    <client-only>
      <video-player ref="videoPlayer"
                    class="vjs-custom-skin"
                    :options="playerOptions"
                    @:playsinline="true"
                         @play="onPlayerPlay($event)"
                         @pause="onPlayerPause($event)"
                         @ended="onPlayerEnded($event)"
                         @loadeddata="onPlayerLoadeddata($event)"
                         @waiting="onPlayerWaiting($event)"
                         @playing="onPlayerPlaying($event)"
                         @timeupdate="onPlayerTimeupdate($event)"
                         @canplay="onPlayerCanplay($event)"
                         @canplaythrough="onPlayerCanplaythrough($event)"
                         @ready="playerReadied"
                         @statechanged="playerStateChanged($event)"/>
    </client-only>
  </div>
</template>

<script>
export default {
  name: "index",
  data() {
    return {
      playerOptions: {
        autoplay: false,
        controls: true,
        sources: [{
            type: 'application/x-mpegurl',
            src: 'https://tomgcs.imgix.video/legacypinata.mov?fm=hls'
        }],
        poster: 'https://tom.imgix.net/legacypinata.png?h=400&auto=format,compress',
        controlBar: {
          timeDivider: false,
          durationDisplay: false
        }
      }
    }
  },
  methods: {
    // listen event
      onPlayerPlay(player) {
        // console.log('player play!', player)
      },
      onPlayerPause(player) {
        // console.log('player pause!', player)
      },
      onPlayerEnded(player) {
        // console.log('player ended!', player)
      },
      onPlayerLoadeddata(player) {
        // console.log('player Loadeddata!', player)
      },
      onPlayerWaiting(player) {
        // console.log('player Waiting!', player)
      },
      onPlayerPlaying(player) {
        // console.log('player Playing!', player)
      },
      onPlayerTimeupdate(player) {
        // console.log('player Timeupdate!', player.currentTime())
      },
      onPlayerCanplay(player) {
        // console.log('player Canplay!', player)
      },
      onPlayerCanplaythrough(player) {
        // console.log('player Canplaythrough!', player)
      },
      // or listen state event
      playerStateChanged(playerCurrentState) {
        // console.log('player current update state', playerCurrentState)
      },
      // player is ready
      playerReadied(player) {
        // seek to 10s
        console.log('example player 1 readied', player)
        player.currentTime(0)
        // console.log('example 01: the player is readied', player)
      }
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