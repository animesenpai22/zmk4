# Advanced ZMK Behaviors Reference

This configuration now includes comprehensive advanced behaviors inspired by [infused-kim's ZMK config](https://github.com/infused-kim/zmk-config). Here's what you can use:

## 🏠 Homerow Mods

### Positional Homerow Mods
- `&hm_l` - Left hand homerow mods (optimized timing)
- `&hm_r` - Right hand homerow mods (optimized timing)
- `&hm_shift_l` - Left shift homerow (faster timing)
- `&hm_shift_r` - Right shift homerow (faster timing)
- `&hm` - Non-positional homerow mods

### Original Homerow Mods (kept for compatibility)
- `&bhml` - Balanced homerow left
- `&bhmr` - Balanced homerow right

## 🔄 Mod Morph Behaviors

### Shift + Key Combinations
- `&mm_shift_caps_word_l/r` - Sticky shift, Shift+tap = Caps Word
- `&mm_bspc_del` - Backspace, Shift+tap = Delete
- `&mm_bspc_del_layer` - Backspace + layer, Shift+tap = Delete
- `&mm_spc_unds_layer` - Space + layer, Shift+tap = Underscore
- `&mm_grave_caret` - Grave, Shift+tap = Caret (^)
- `&mm_plus_minus` - Plus, Shift+tap = Minus
- `&mm_comma_semi_meh` - Comma, Shift+tap = Semicolon
- `&mm_dot_colon` - Dot, Shift+tap = Colon

### Navigation with CMD Modifiers
- `&mm_none_undo` - None, CMD+tap = Undo
- `&mm_left_word_cut` - Left word, CMD+tap = Cut
- `&mm_up_save` - Up arrow, CMD+tap = Save
- `&mm_down_copy` - Down arrow, CMD+tap = Copy
- `&mm_none_paste` - None, CMD+tap = Paste

### Number Layer Shortcuts
- `&mm_1_cut` - 1, CMD+tap = Cut
- `&mm_2_copy` - 2, CMD+tap = Copy
- `&mm_5_save` - 5, CMD+tap = Save

### Escape/Grave Behaviors
- `&mm_grescm` - Escape, Shift+tap = Grave
- `&mm_grescm_gui` - Escape + GUI, Shift+tap = Grave

### Auto-Pairing Brackets
- `&mm_bracket_r` - (, Shift+tap = )
- `&mm_bracket_sq` - [, Shift+tap = ]
- `&mm_bracket_c` - {, Shift+tap = }
- `&mm_bracket_a` - <, Shift+tap = >

## 🕺 Tap Dance Behaviors

### Advanced Shift
- `&td_shift_l` - Left Shift / Caps Word / Caps Lock
- `&td_shift_r` - Right Shift / Caps Word / Caps Lock

### Layer Control
- `&td_num_layer` - Tap=DEL, Hold=NUM layer, Double-tap=Toggle NUM
- `&td_nav_layer` - Complex navigation layer control
- `&td_sym_layer` - Complex symbol layer control

### Bluetooth
- `&td_out_bt_clear` - Toggle output, Double-tap = Clear BT

### Email
- `&td_at_email` - @ / Personal Email / Work Email

## 🎯 Auto Mod & Auto Shift

### Auto Mod
Use `AM(hold, tap)` macro:
```
AM(RPAR, LPAR)  // Tap: (, Hold: )
```

### Auto Shift
Use `AS(key)` macro:
```
AS(A)  // Tap: a, Hold: A
```

## 📧 Macros

### Email Macros
- `&email` - Your personal email
- `&m_type_email_p` - Advanced personal email
- `&m_type_email_w` - Work email template
- `&anime_name` - Anime name template

### Text Expansion
- `&m_type_md_code_block` - Markdown code block
- `&m_select_all` - Select all shortcut
- `&m_undo` - Undo macro
- `&m_redo` - Redo macro

### System
- `&m_screenshot` - macOS screenshot
- `&m_spotlight` - macOS Spotlight search

## 🔧 Utility Behaviors

### Layer Control
- `&ltog` - Layer toggle with hold-tap
- `&sklt` - Sticky key layer tap
- `&my_safe_hold_tap` - Original safe hold-tap

### Email Behaviors
- `&ht_type_email` - Hold for email, tap for key
- `&td_at_email` - Tap dance @ and emails

## 🎹 How to Use

### Example Usage in Keymap:
```devicetree
&hm_l LGUI A          // Hold for LGUI, tap for A (left hand)
&mm_shift_caps_word_l // Tap for sticky shift, Shift+tap for caps word
&td_shift_r          // Tap for shift, double-tap for caps word, triple for caps lock
AM(RPAR, LPAR)       // Tap for (, hold for )
AS(A)                // Tap for a, hold for A
&mm_bspc_del         // Tap for backspace, Shift+tap for delete
```

### Navigation Layer Example:
```devicetree
&mm_left_word_cut    // Left word jump, CMD+tap for cut
&mm_up_save          // Up arrow, CMD+tap for save
&mm_down_copy        // Down arrow, CMD+tap for copy
```

## ⚙️ Configuration

### Timing Settings:
- `HM_TAPPING_TERM = 300ms` - Normal homerow mod timing
- `HM_TAPPING_TERM_FAST = 200ms` - Fast timing for shifts
- `HM_PRIOR_IDLE = 150ms` - Prior idle requirement
- `TD_TAPPING_TERM = 300ms` - Tap dance timing

### Key Shortcuts:
- `MY_UNDO` = `LG(Z)` - macOS/Linux undo
- `MY_COPY` = `LG(C)` - macOS/Linux copy
- `MY_PASTE` = `LG(V)` - macOS/Linux paste
- `MY_CUT` = `LG(X)` - macOS/Linux cut

## 🚀 Benefits

1. **Reduced finger movement** with homerow mods
2. **Context-aware shortcuts** with mod morphs
3. **Multi-function keys** with tap dance
4. **Smart bracket pairing** 
5. **Quick text expansion**
6. **Efficient layer switching**
7. **Platform-aware shortcuts**

Your keymap now has professional-grade functionality similar to high-end custom keyboards!
