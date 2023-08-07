# Cleaning_folder

This script is designed to sort and arrange files in the specified folder. The script goes through the transfer during the request call and sorts all files into groups: images ('JPEG', 'PNG', 'JPG', 'SVG'); video files ('AVI', 'MP4', 'MOV', 'MKV'); documents('DOC', 'DOCX', 'TXT', 'PDF', 'XLSX', 'PPTX'); music ("MP3", "OGG", "WAV", "AMR"); archives ('ZIP', 'GZ', 'TAR'); unknown extensions.

According to the results of work determine: List of files in each category (music, video, photo, etc.) List of all known script extensions that meet in the target folder. A list of all extensions that are unknown to the script.

Next: Images are transferred to the images folder documents documents audio files are transferred to audio video files in video archives are unpacked and their contents are transferred to the files files files unknown

All files and folders are renamed using the normalize function. file extensions are not changed after renaming. empty folders deleted script ignores folders archives, video, audio, documents, images, unknown; decompressed archive content is transferred to a folder archive subfolder named just like the archive, but without extension at the end; files whose extensions are unknown, remain unchanged.
