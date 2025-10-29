# f3-tulsa-emojis
Collection of Tulsa-related F3 emojis; just wanted a place to dump all emojis when moving them to the new Tulsa Scissortail region.

# Export/Import
1. Followed steps here to export: [The How to bulk download Slack emojis](https://medium.com/@alexleybourne/the-how-to-bulk-download-slack-emojis-33cdd6e70eb0)
1.  PowerShell to name emoji files correctly:
    ```
    cd '~\Downloads\f3ttown.slack.com\emoji.slack-edge.com\T03KJ2JQ3JT' # change to actual directory name
    ls -Directory | %{ dir "$($_.FullName)" -File } | %{ copy -Verbose -Path $_.FullName -Destination "~\Pictures\Slack\f3ttown-export\$($_.Directory.BaseName)$($_.Extension)" } # change to actual export path
    ```
2. [Chrome extension to allow uploading in bulk](https://chromewebstore.google.com/detail/neutral-face-emoji-tools/anchoacphlfbdomdlomnbbfhcmcdmjej) 
