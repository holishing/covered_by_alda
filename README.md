# Melody test covered by alda music

## Requirement
- [Alda](https://alda.io)
- [Timidity++](https://sourceforge.net/projects/timidity/): Optional, If you want to export music to more format.

## Play 
```
alda play -f shojo_rei.alda
```

## Export to Midi Music
```
alda export -f shojo_rei.alda -o shojo_rei.midi
```

## Export to AAC/MP3 format by MIDI

```
timidity shojo_rei.midi  -Ow -o - | ffmpeg -i - -acodec mp3 shojo_rei.mp3
timidity shojo_rei.midi  -Ow -o - | ffmpeg -i - -acodec aac shojo_rei.aac
```

## Material
- [Shojo Rei](https://youtu.be/JW3N-HvU0MA)
