# ABCcz

A macOS keyboard layout: US ABC with Czech letters on the Option key.
Made with [Ukelele](https://software.sil.org/ukelele/).

## Layout

Without Option, it types like the standard US ABC layout.

With Option, the number row gives Czech letters, in the same spots as the Czech keyboard:

| Key | Option | Shift + Option |
| --- | ------ | -------------- |
| 2   | ě      | Ě              |
| 3   | š      | Š              |
| 4   | č      | Č              |
| 5   | ř      | Ř              |
| 6   | ž      | Ž              |
| 7   | ý      | Ý              |
| 8   | á      | Á              |
| 9   | í      | Í              |
| 0   | é      | É              |
| [   | ú      | Ú              |
| ;   | ů      |                |

Dead keys for the rest:

- `Option =`, then a letter: acute (´), e.g. `ó`, `Ó`.
- `Shift Option =`, then a letter: caron (ˇ), e.g. `ď`, `ť`, `ň`.

## Install

1. Get the files: `git clone https://github.com/hedai7/ABCcz.git`, or download the ZIP from GitHub and unzip it.
2. Copy `ABCcz.bundle` to `~/Library/Keyboard Layouts/`:

   ```sh
   cp -R ABCcz/ABCcz.bundle ~/Library/Keyboard\ Layouts/
   ```

   To install it for all users, copy it to `/Library/Keyboard Layouts/` instead (needs `sudo`).
3. Log out and log back in.
4. Open **System Settings → Keyboard → Text Input → Input Sources → Edit**.
5. Click **+**, find **ABCcz** (usually under **Others**), and click **Add**.
6. Pick **ABCcz** from the input menu in the menu bar.

If macOS does not show the layout, remove the download quarantine flag and log in again:

```sh
xattr -dr com.apple.quarantine ~/Library/Keyboard\ Layouts/ABCcz.bundle
```

## Uninstall

1. Remove **ABCcz** in **Input Sources**.
2. Delete `~/Library/Keyboard Layouts/ABCcz.bundle`.
3. Log out and log back in.

## License

[MIT](LICENSE)
