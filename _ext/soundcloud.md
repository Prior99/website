---
title: Mopidy-SoundCloud
service: SoundCloud
logo: /media/ext/soundcloud.png
type: backend
dev:
  github: mopidy/mopidy-soundcloud
  circleci: true
  codecov: true
dist:
  pypi: Mopidy-SoundCloud
  apt-debian: mopidy-soundcloud
  apt-mopidy: mopidy-soundcloud
  arch-aur: mopidy-soundcloud
  homebrew:
    tap: mopidy/mopidy
    formula: mopidy-soundcloud
oauth:
  button:
    style: "background-color: #FF3300; color: #FFF"
    logo:
      url: https://unpkg.com/simple-icons@latest/icons/soundcloud.svg
      style: "filter: invert(1)"
  endpoint: https://secure.soundcloud.com/connect?client_id=93e33e327fd8a9b77becd179652272e2&scope=non-expiring&response_type=code_and_token&redirect_uri=https://www.mopidy.com/soundcloud_callback
  origin: https://mopidy.com
  config:
    soundcloud:
      - auth_token
---

A backend for playing music from the
[SoundCloud](https://soundcloud.com/) service.
