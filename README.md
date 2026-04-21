================================================================================
                     DragON - Windows Gesture Login
                          Trial Version Readme
================================================================================

Thank you for trying DragON. This document covers everything you need to get
started with the trial version.

For full online documentation visit: www.techporch.com


================================================================================
WHAT IS DragON ?
================================================================================

DragON is a Windows credential provider that replaces your password with a
visual drag-and-drop gesture. Instead of typing, you authenticate by dragging
icons across a themed image grid at the Windows login or lock screen.

It works alongside your existing Windows login methods — your password and PIN
remain available at all times. DragON simply adds a faster, more visual way
to sign in.

Ideal for:
  - Touchscreen devices and tablets where typing is cumbersome
  - Users who prefer visual / spatial memory over text passwords
  - Accessibility scenarios


================================================================================
TRIAL VERSION LIMITATIONS
================================================================================

The trial version is fully functional with the following restrictions:

  - Maximum 1 drag sequence per login  (full version: up to 8)
  - Maximum 1 enrolled user account    (full version: unlimited)
  - 2 image themes available           (full version: all 5 themes)
  - Trial period: 180 days from installation

To remove all restrictions, purchase the full version at www.techporch.com.


================================================================================
WHAT'S INCLUDED
================================================================================

  dragEnroll.exe    Enrollment application — run this once to set up your
                    drag sequence. Requires administrator privileges.

  dragVerify.exe    Verification UI — launched automatically at login.
                    Do not run this directly.

  dragSupp.dll      Support library — required by both applications.
                    Do not delete or move this file.

  dragProv.dll      Windows credential provider — registered during install.
                    Do not delete or move this file.

  Assets\           Image theme files used during login.

  Readme.txt        This file.


================================================================================
STEP 1 — ENROLLMENT  (one-time setup)
================================================================================

Enrollment registers your drag sequence with DragON. You only need to do
this once per user account.

  1. Launch dragEnroll.exe from the DragON installation folder.
     (Right-click -> Run as administrator if prompted.)

  2. Enter your Windows credentials:
       - User Name       (your Windows account name)
       - Domain / PC     (auto-populated — leave as is for local accounts)
       - Password        (your current Windows login password)
       - Reenter Password
     If you use a Microsoft / Live account, check "I am a Windows Live User"
     and enter your Microsoft account email instead.
     Click Next.

  3. DragON validates your credentials against Windows. If validation fails,
     double-check that Caps Lock is off and your password is correct.

  4. Select a theme for your tile grid. The theme determines the images you
     will drag at every future login. Available themes in the trial:
       - Animals     Illustrated animals from around the world
       - Landmarks   Famous landmarks: Eiffel Tower, Taj Mahal, and more

  5. Create your drag sequence:
       - Click a tile to set your START TILE (shown in the left panel).
       - Click a different tile to set your END TILE.
       - The LED indicator turns GREEN when both tiles are chosen.

     TIP: Pick tiles that are personally meaningful and easy to remember,
     but not obvious to someone who knows you.

  6. Click Next to verify your sequence:
       - Drag from your Start Tile to your End Tile to confirm.
       - If you make a mistake, start the verification from the beginning.
         There is no time limit.

  7. Click Done. Enrollment is complete. You can now use DragON to log in.

  NOTE (Trial): Only 1 drag sequence is supported. The full version allows
  up to 8 sequences chained together for stronger security.


================================================================================
STEP 2 — LOGGING IN
================================================================================

After enrollment, DragON appears as a sign-in option on the Windows login
and lock screen (Windows key + L).

  1. At the login screen, select DragON from the sign-in options.
     The DragON verification window opens.

  2. Click the theme icon at the top of the grid that matches the theme
     you chose during enrollment. The grid will update to show those images.

     WARNING: You must select the same theme used during enrollment.
     Selecting a different theme shows different tiles and your drag will
     not match.

  3. Find your Start Tile. Click, hold, and drag to your End Tile, then
     release. This must exactly match what you set up during enrollment.

  4. If the drag is correct, Windows logs you in immediately.
     If you make a mistake, the screen resets and you can try again.
     There is no time limit and no lockout for incorrect attempts.

  5. To cancel DragON and return to standard Windows login at any time,
     click the back-arrow (arrow icon) in the top-left corner of the
     verification screen. Your Windows password, PIN, and any other
     configured sign-in methods remain available.


================================================================================
STEP 3 — IF YOU CHANGE YOUR WINDOWS PASSWORD
================================================================================

If you change your Windows password after enrollment, DragON will detect this
the next time you log in. Your drag sequences are NOT affected — only the
stored password needs to be updated. No re-enrollment is required.

What happens:

  1. Log in using DragON as normal. Perform your drag sequence.
     DragON validates your drag sequences successfully.

  2. Windows reports "The user name or password is incorrect."
     This is EXPECTED — it means DragON used the old stored password.
     Click OK.

  3. DragON displays a password update screen:
       "Your password has been changed. Please provide your new password
        and validate your identity by dragging Start Tile to End Tile."

  4. Enter your new Windows password in the New Password and
     Reenter New Password fields.

  5. Perform your drag sequence again to confirm your identity.

  6. DragON updates its stored credentials and Windows logs you in.
     All future logins will use the new password automatically.


================================================================================
TROUBLESHOOTING
================================================================================

  Problem                          Solution
  -------                          --------
  Credential validation fails      Check your username and password. Ensure
  during enrollment                Caps Lock is off. Verify the domain or
                                   computer name is correct.

  Forgot which tiles you chose     Click the back-arrow to return to the
  at login                         standard Windows login screen. Sign in
                                   with your password or PIN, then re-run
                                   dragEnroll.exe to update your enrollment.

  Wrong drag during verification   The screen resets automatically. Start
                                   again from your first sequence. No need
                                   to re-enroll.

  DragON tile not visible at       Ensure dragProv.dll is correctly registered.
  the login screen                 Re-run the installer to repair the
                                   installation.

  "Incorrect password" keeps       Make sure you are entering your NEW Windows
  appearing during pwd update      password, not the old one. Both fields must
                                   match your current Windows password exactly.

  DragON does not prompt for       At the login screen, click sign-in options
  password update                  and select DragON as the active provider.


================================================================================
UNINSTALLING DragON
================================================================================

Use Add/Remove Programs (Windows Settings -> Apps) to uninstall DragON.
This removes the credential provider and all associated files. Your Windows
password and other sign-in methods are not affected.


================================================================================
SUPPORT & UPGRADE
================================================================================

  Website:   www.techporch.com
  Support:   www.techporch.com/contact

  To purchase the full version and unlock all themes, up to 8 drag sequences,
  and unlimited user enrollments, visit www.techporch.com/products.


================================================================================
                   Copyright (c) Techporch. All rights reserved.
================================================================================
