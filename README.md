# find

## find multiple files and copy them into folder

### $ find . -type f `\`( -name "*smth.jpg" -o -name "*onemore.jpeg" -o -name "*sometype" `\`) -exec cp "{}" /path/to/folder `\`;

## find all webm files that are in the current directory and in all sub-folders and extract the audio to mp3 format.

### $ find . -type f -iname "*.webm" -exec bash -c 'FILE="$1"; ffmpeg -i "${FILE}" -vn -ab 128k -ar 44100 -y "${FILE%.webm}.mp3";' _ '{}' \;
