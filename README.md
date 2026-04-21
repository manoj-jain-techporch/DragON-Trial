# DragON — Windows Gesture Login
### Trial Version

**DragON** is a Windows credential provider that replaces your password with a visual drag-and-drop gesture. Instead of typing, you authenticate by dragging icons across a themed image grid at the Windows login or lock screen.

It works alongside your existing sign-in methods — your password and PIN remain available at all times.

> **Full documentation:** [www.techporch.com](https://www.techporch.com)

---

## What Is DragON?

DragON turns the Windows lock screen into a visual puzzle. During setup you pick a **Start Tile** and an **End Tile** from a themed image grid. At every login you simply drag from one to the other — no typing required.

**Ideal for:**
- Touchscreen devices and tablets where typing is cumbersome
- Users who prefer visual / spatial memory over text passwords
- Accessibility scenarios

---

## Trial Version Limitations

> ⏱ The trial version is fully functional for **180 days** from installation with the following restrictions.

| Feature | Trial | Full Version |
|---|---|---|
| Drag sequences per login | 1 | Up to 8 |
| Enrolled user accounts | 1 | Unlimited |
| Image themes | 2 (Animals, Landmarks) | 5 |
| Trial period | 180 days | Unlimited |

Upgrade at [www.techporch.com/products](https://www.techporch.com/products) to remove all restrictions.

---

## What's Included

| File | Description |
|---|---|
| `dragEnroll.exe` | Enrollment app — run once to set up your drag sequence. Requires administrator privileges. |
| `dragVerify.exe` | Verification UI — launched automatically at login. Do not run directly. |
| `dragSupp.dll` | Support library required by both applications. Do not delete or move. |
| `dragProv.dll` | Windows credential provider registered during install. Do not delete or move. |
| `Assets\` | Image theme files used during login. |
| `README.md` | This file. |

---

## Step 1 — Enrollment (One-Time Setup)

Enrollment registers your drag sequence with DragON. You only need to do this once per user account.

1. **Launch `dragEnroll.exe`** from the DragON installation folder.
   *(Right-click → Run as administrator if prompted.)*

2. **Enter your Windows credentials:**
   - **User Name** — your Windows account name
   - **Domain / PC** — auto-populated; leave as-is for local accounts
   - **Password** — your current Windows login password
   - **Reenter Password**

   If you use a Microsoft / Live account, check *"I am a Windows Live User"* and enter your Microsoft account email instead. Click **Next**.

3. **Credential validation** — DragON validates your credentials against Windows. If this fails, ensure Caps Lock is off and your password is correct.

4. **Select a theme** for your tile grid. The theme determines the images you will drag at every future login.

   | Theme | Description |
   |---|---|
   | Animals | Illustrated animals from around the world |
   | Landmarks | Famous landmarks: Eiffel Tower, Taj Mahal, and more |

5. **Create your drag sequence:**
   - Click a tile to set your **Start Tile** (shown in the left panel)
   - Click a different tile to set your **End Tile**
   - The LED indicator turns **green** when both tiles are chosen

   > 💡 **Tip:** Pick tiles that are personally meaningful and easy to remember, but not obvious to someone who knows you.

6. **Verify your sequence** — drag from your Start Tile to your End Tile to confirm. If you make a mistake, restart verification from the beginning. There is no time limit.

7. Click **Done**. Enrollment is complete. You can now use DragON to log in.

> ⏱ **Trial:** Only 1 drag sequence is supported. The full version allows up to 8 sequences chained together for stronger security.

---

## Step 2 — Logging In

After enrollment, DragON appears as a sign-in option on the Windows login and lock screen (**Windows key + L**).

1. At the login screen, **select DragON** from the sign-in options. The DragON verification window opens.

2. **Select your theme** — click the theme icon at the top of the grid that matches the theme you chose during enrollment.

   > ⚠️ **Warning:** You must select the same theme used during enrollment. A different theme shows different tiles and your drag will not match.

3. **Perform your drag** — locate your Start Tile, click and hold, drag to your End Tile, then release. This must exactly match your enrollment.

4. If the drag is correct, **Windows logs you in immediately**. If you make a mistake, the screen resets and you can try again. There is no time limit and no lockout for incorrect attempts.

5. To **cancel DragON** and return to standard Windows login at any time, click the **back-arrow (↩)** in the top-left corner. Your Windows password, PIN, and all other configured sign-in methods remain available.

---

## Step 3 — If You Change Your Windows Password

If you change your Windows password after enrollment, DragON detects this the next time you log in. **Your drag sequences are not affected** — only the stored password needs updating. No re-enrollment is required.

1. **Log in using DragON as normal.** Perform your drag sequence. DragON validates it successfully.

2. **Windows reports** *"The user name or password is incorrect."*
   This is **expected** — DragON used the old stored password. Click **OK**.

3. **DragON displays a password update screen:**
   > *"Your password has been changed. Please provide your new password and validate your identity by dragging Start Tile to End Tile."*

4. Enter your **new Windows password** in both the New Password and Reenter New Password fields.

5. **Perform your drag sequence again** to confirm your identity.

6. DragON updates its stored credentials and Windows logs you in. All future logins use the new password automatically.

---

## Troubleshooting

| Problem | Solution |
|---|---|
| Credential validation fails during enrollment | Check your username and password. Ensure Caps Lock is off and the correct domain or computer name is entered. |
| Forgot which tiles you chose at login | Click the back-arrow (↩) to return to standard Windows login. Sign in with your password or PIN, then re-run `dragEnroll.exe` to update your enrollment. |
| Wrong drag during verification | The screen resets automatically. Start again from your first sequence. No re-enrollment needed. |
| DragON tile not visible at the login screen | Ensure `dragProv.dll` is correctly registered. Re-run the installer to repair the installation. |
| "Incorrect password" keeps appearing during password update | Make sure you are entering your **new** Windows password, not the old one. Both fields must match your current Windows password exactly. |
| DragON does not prompt for password update | At the login screen, click sign-in options and select DragON as the active provider. |

---

## Uninstalling DragON

Go to **Windows Settings → Apps** and uninstall DragON. This removes the credential provider and all associated files. Your Windows password and other sign-in methods are not affected.

---

## Support & Upgrade

- **Website:** [www.techporch.com](https://www.techporch.com)
- **Support:** [www.techporch.com/contact](https://www.techporch.com/contact)

Upgrading unlocks all 5 themes, up to 8 drag sequences per login, and unlimited user enrollments.

---

*Copyright &copy; Techporch. All rights reserved.*
