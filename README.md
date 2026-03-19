# Stream.Transcripts
Gigaohm Biological High Resistance Low Noise Information Transcripts

The purpose of this repo is to place AI generate captions in one location for easy searching. How this repo will change will depend on how well it is working for our purposes.

**Note:** *Due to when this repo got created, it would not be possible to generate all the captions for all the streams (at least initially). JC has his own archive of all the streams, so this is possible, but it is a matter of time and effort.*

_Update (2026-03-19)_:
- In the 2025-11-05 stream (not yet committed), I noticed that many words were dropped in the transcription compared to in the actual stream (probably due to a very old Whisper snapshot I'm using).
    - I was planning on fixnig that, but never got around to it.
    - Going forward, any more transcripts will be more like that where I have basically done no QC at all.
    - However, this is probably not a big loss as there has been zero people who have pinged me about this repo.
    - Therefore it's probably more functionally just and old archive at this point.
    - There will be future transcriptions as they already have been done, just that I have not had the time to create the commits. 
 
        ~ _Management_

## Organization

All transcripts will be
- [twitch](twitch) - from https://twitch.tv/gigaohmbiological
    - Due to legacy reasons, streams are still organized around Twitch IDs, but the captions for more recent streams may be generated from other sources.
        - Peertube - from https://stream.gigaohm.bio
        - Rumble - from https://rumble.com/user/GigaohmBiological
- [youtube](youtube) - from [JC on a Bike (channel)](https://www.youtube.com/@JConabike)
- [guest.speaking](guest.speaking) - from various

Other folders:
- [tools](tools) - tools and scripts

### Conventions

In each transcript "top" folder, will be a new folder for each stream. These folders will typically start with the stream ID and include the title and date of ths stream. Inside each folder will be the transcript (probably in [VTT format](https://developer.mozilla.org/en-US/docs/Web/API/WebVTT_API)). This provides some flexibility in case we need to put additional files there. It will also have a ReadMe.md file which should include some information like a link back to the known streams.

# Plans

Initially this will server as a repository for AI generated (and corrected) transcripts from any streams that Gigaohm Biological appears for the purpose of searching. However, over time, we might develop new capabilities.

## Javascript + Static Site

One idea is to generate (using github pages) a static site using javascript and pre-built indexes to make the searching a lot better/easier (including hot-linking to the right timestamp from either the Twitch or alternative sourced stream). This would make finding the content that one wants to share much faster.

(This is a far-off-in-the-future plan...)
