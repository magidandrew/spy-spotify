# [How is this fork different?](#how-its-different)
Spytify allows you to not redownload tracks that already exist in your library. Even though Spytify won't record, Spotify will continue playing the track which will result in wasted time. This fork skips the tracks on Spotify if they have already been recorded, ensuring that Spotify is always downloading music that doesn't exist in your library.

Modified binary can be downloaded from the [releases page](https://github.com/magidandrew/spy-spotify-with-skipping/releases). However, feel free to build from source from the `.sln` file. The diff from the original repository is only a few lines.

### ...The Rest of the Spytify Description From Spytify Repo...

Spytify is a Spotify recorder for Windows which records Spotify audio without recording or playing ads, ensuring no loss in sound quality. It automatically splits songs into separate tracks and records to MP3 with media metadata, meaning you can easily start enjoying your music offline.

<p align="center"><img alt="Spotify Recorder logs" src="https://jwallet.github.io/spy-spotify/assets/images/ui_record.png" /></p>

### [How does it work?](#how-does-it-work)

Spytify records what Spotify outputs, which is a longer process than downloading a Spotify playlist with a tool.

However, Spytify ensures that all tracks will be the official released one, all sound volume normalized and with media tags and album cover. Playlist Downloaders get mostly all tracks from YouTube which means that they can't guarantee the choosen track will fit 100% the one in your playlist and they will all be the same quality.

Spytify records the same quality that Spotify outputs ([Spotify Free 160kbps, Spotify Premium 320kbps](https://support.spotify.com/us/article/audio-quality/)), so the recorded copy will be indistinguishable from Spotify’s one.

### [How to install it?](#how-to-install-it)

Follow the steps shown in the F.A.Q section : [_How to install Spytify?_](https://jwallet.github.io/spy-spotify/faq.html#install-spytify)

### [How to use it?](#how-to-use-it)

A standard use is to start a recording session using your favorite playlist and let it record overnight, so you avoid waiting for it to end, because Spytify does not download but records. You will then get all your songs automatically split into separate tracks without ads and with metadata.

A recorder requires a good sound card to be able to record good quality, that's why Spytify comes with a Virtual Audio Cable device, if you have issues with your sound card (volume slider and other apps sound affects the recordings, or overall recorded sound quality is worst than Spotify) you can install this virtual device using the **Speakers+** icon in Spytify settings.

Don't forget to hit the [F.A.Q.](https://jwallet.github.io/spy-spotify/faq.html) for tips on:

- [_How to install Virtual Audio Cable device for better recording quality?_](https://jwallet.github.io/spy-spotify/faq.html#install-better-audio-endpoint-device)
- [_How to isolate Spytify and Spotify on a virtual audio device to avoid background noises?_](https://jwallet.github.io/spy-spotify/faq.html#isolate-spotify-audio-endpoint)
- [_How to reroute sound/output of a virtual audio device to my main audio device to listen to it?_](https://jwallet.github.io/spy-spotify/faq.html#listen-to-virtual-device)
- [_How to connect to Spotify API for more accurate media tags?_](https://jwallet.github.io/spy-spotify/faq.html#media-tags-not-found)


### [App features](#app-features)

|                                                                        |         Feature         | Description                                                                                                                                                                                         |
| ---------------------------------------------------------------------- | :---------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <img alt="features" src="https://jwallet.github.io/spy-spotify/assets/images/feature_no_ad.png" />         |       **No Ads**        | Mutes and doesn't record audio ads.                                                                                                                                                                  |
| <img alt="features" src="https://jwallet.github.io/spy-spotify/assets/images/feature_mute_apps.png" />     |  **Mutes Other Apps**   | Mutes any other applications while spying Spotify. Both apps can be [isolated in a their own audio endpoint device](https://jwallet.github.io/spy-spotify/faq.html#isolate-spotify-audio-endpoint) to record better audio quality.      |
| <img alt="features" src="https://jwallet.github.io/spy-spotify/assets/images/feature_audio_quality.png" /> | **Great Audio Quality** | Gets and records with the same great audio quality as Spotify, when your [Spotify audio quality](https://jwallet.github.io/spy-spotify/faq.html#maximize-quality-spotify-settings) is optimal.                                          |
| <img alt="features" src="https://jwallet.github.io/spy-spotify/assets/images/feature_max_out.png" />       |  **Normalize volume**   | Normalize by adjusting the volume to the level originally delivered by Spotify for Spotify and Spytify when the recording session starts (keep the **Normalize** feature `ON` in Spotify settings). |

### [File features](#file-features)

- Splits the recorded sound into individual tracks using the artist and track names as the title, like so:
  - `Artist - Track.mp3`
- Saves all recordings under the same path:
  - `../My Music/`
- Automatically adds metadata from Last.fm (or [Spotify API](https://jwallet.github.io/spy-spotify/faq.html#media-tags-not-found)) to .mp3 file:
  - \# track
  - Track Title
  - Artist
  - Album Title
  - Album Art Cover
  - Genre

<p align="center"><img alt="Recorded songs with album cover and media tags in Windows Explorer" src="https://jwallet.github.io/spy-spotify/assets/images/saved_songs_list.png" /></p>

### [Requirements](#requirements)

Spytify runs on Windows only.

- Microsoft Framework ([.NET 4.6.1](https://www.microsoft.com/en-ca/download/details.aspx?id=49981) or higher).
- Spotify Desktop application.

A **free Spotify account** will work, but Spotify restricts audio quality to 160 kbps. Having a Premium Spotify subscription will enable recording of up to 320 kbps audio.
