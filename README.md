# Claude social posting

Drop videos here and Claude uploads them to PostEverywhere, writes the caption, and schedules the post after you approve it.

## How to drop a video

1. Open the folder for the account the video is for:
   - [inbox/cosmiccellfoods](inbox/cosmiccellfoods)
   - [inbox/cwbotanics](inbox/cwbotanics)
   - [inbox/cwbotanicshealth](inbox/cwbotanicshealth)
   - [inbox/cwbotanicalhealth](inbox/cwbotanicalhealth) (reconnect this account in PostEverywhere first)
2. Click **Add file → Upload files**, drag the video in, and click **Commit changes**.
3. Tell Claude in chat: "new videos in the inbox". Add any notes (what it's about, when to post).

**File rules:** MP4, vertical 9:16 for Reels. The GitHub website takes files up to 25 MB; GitHub Desktop or git takes up to 100 MB.

Optional: put a `.txt` file with the same name next to the video (e.g. `promo1.mp4` + `promo1.txt`) with notes or a caption you want used.

## What's where

| Folder | Holds |
| --- | --- |
| `inbox/<account>/` | Videos waiting to be posted |
| `accounts/<account>/voice.md` | Brand voice for that account. Every caption follows it |
| `accounts/accounts.json` | PostEverywhere account IDs |
| `posted/` | Log of what was scheduled, with captions and times |

Once a video is scheduled, Claude moves it out of the inbox and logs it in `posted/`.
