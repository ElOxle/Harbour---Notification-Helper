# Harbour - Notification Helper

`Harbour - Notification Helper` is an optional companion app for [Harbour](https://apps.apple.com/) on macOS.

It is not required to use Harbour.

The Mac App Store version of Harbour works on its own. This helper simply adds one extra capability for people who want it: it lets Harbour detect notification badges in the Dock and reflect that in Harbour’s UI.

## What It Does

When installed, the helper can:

- read Dock app badge state on your Mac
- detect which apps currently show a notification badge
- pass that information to Harbour
- let Harbour highlight those apps and show unread counts

This means Harbour can show things like:

- apps with notifications in red
- badge counts next to app names
- a menu bar alert state when Dock notifications are active

## Important

This helper is:

- completely optional
- separate from the Mac App Store app
- not needed for Harbour’s normal operation

If you do not install it, Harbour will still work normally. You simply will not get Dock notification integration.

## Why Is It Separate?

Harbour is distributed through the Mac App Store.

This helper is distributed separately because it performs system-level Dock inspection that is outside the scope of the App Store version. Keeping it separate ensures:

- the App Store app remains clean and self-contained
- users can choose whether they want this extra functionality
- installation is explicit and under the user’s control

## Requirements

- macOS
- Harbour installed
- Accessibility permission granted to the helper

## Installation

1. Download `Harbour - Notification Helper`
2. Move it to `/Applications`
3. Open Harbour
4. In Harbour Settings, go to `Dock Notifications`
5. Enable Dock Notifications
6. If prompted, grant Accessibility access to the helper

## Permissions

The helper may request:

- **Accessibility**  
  This is used to inspect Dock badge information so Harbour can reflect notification state.

The helper does not replace Harbour, and it does not need to be opened manually during normal use.

## Notes

- Launch the helper through Harbour, not by opening it directly
- If you open it manually, it may simply show a message or quit
- Harbour will detect it automatically once installed

## Troubleshooting

If Harbour does not show Dock notifications:

1. Confirm the helper is installed in `/Applications`
2. Open Harbour Settings → `Dock Notifications`
3. Check that the helper is detected
4. Confirm Accessibility permission has been granted
5. Use `Refresh Now` in Harbour Settings

## Disclaimer

This project is an optional helper for Harbour and is provided outside the Mac App Store. It is intended only to extend Harbour with Dock notification badge support.
