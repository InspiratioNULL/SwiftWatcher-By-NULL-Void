# SwiftWatcher-By-NULL-Void

## Why Choose SwiftWatcher?

Say goodbye to overpriced, unreliable, rip off dusters named after shrubs and iBalls.  SwiftWatcher is here, and all eye colors are welcome! 🟢🔵⚫⚪️🟤

### Key Features:
- **One Executable, One Process:** Minimal CPU usage, even when running multiple flags. Call it as many times as you need without breaking a sweat.
- **Unmatched Automation:** Add options for better, faster, and smarter automations as you go.
- **Better Mac Performance:** No dumb helper apps, startup items, or background apps clogging your system. Just one executable doing the job.
- **Transparent Operations:** Want to know what's happening? Just open up the terminal—no mysterious waiting times or shady background processes.

### Uncompromising Reliability:
- **Control Over Timing:** Specify exactly how long *after* an item *is modified* before taking action—whether that’s **5 seconds**, **5 minutes**, or an epic **669 hours**. You’re in charge.
- **Data Safety First:** Rest easy knowing your files won’t be corrupted, moved, copied, or otherwise tampered with until write operations are fully complete.
  
### For The Future:
- **As of right now, Only Apple Silicon is supported, Intel support will be added soon. Updates are going to be added here, star the repo to stay tuned! GUI will be underway, but it will be a separate executable altogether**

### Oh, and Did We Mention?
- **Free as F***:** That’s right. No ridiculous price tags. Just pure, unfiltered utility.



## USAGE:
```USAGE: swiftwatcher --dir-path-string <dir-path-string> [--out-path-string <out-path-string>] [--min-age-string <min-age-string>] [--move <move> ...] [--copy <copy> ...] [--trash <trash> ...] [--rename-pattern <rename-pattern> ...] [--rename-to <rename-to> ...]

OPTIONS:
  -d, --dir-path-string <dir-path-string>
                          The directory to watch.
  -o, --out-path-string <out-path-string>
                          The default output directory for move/copy operations.
  -t, --min-age-string, --min-age <min-age-string>
                          Minimum age impo file before processing (e.g., '10s' for 10 seconds,
                          '5m' for 5 minutes, '1h' for 1 hour). Checks against modification date.
                          If not specified, files are processed after a short stability delay.
  --move <move>           Patterns of files to move. Files are moved to the --out directory.
                          Remember to quote patterns with wildcards (e.g., "*.mp3").
  --copy <copy>           Patterns of files to copy. Files are copied to the --out directory.
                          Remember to quote patterns with wildcards.
  --trash <trash>         Patterns of files to move to Trash. Remember to quote patterns with
                          wildcards.
  --rename-pattern <rename-pattern>
                          Patterns of files to rename (e.g., "*.txt", "document.pdf"). Remember to
                          quote patterns with wildcards.
  --rename-to <rename-to> New extensions for corresponding --rename-pattern files (e.g., "bak",
                          "doc"). Do not include the dot.
  -h, --help              Show help information.
```
## Example
```
swiftwatcher -d /path/to/dir/ -o /path/will/be/created/if/it/doesnt/exist -t 20s --move "*.jpg" "*.png" "*.gif" "*.webp" --copy "*.txt" "*.pdf" "*.md" --rename-pattern "*.mp4" --rename-to "*.mp3" --trash "*.wav" "*.bmp" "*.html"
```
## Example 2 
```
swiftwatcher -d /path/to/dir/ -o /path/to/dir -t 1m --trash "*.mp4" --move "*.mp3"
```


