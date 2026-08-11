# Learnings

> Getting to know my sofle


## Issue: Keymap not working

Left and right thumb buttons mapped to space and enter were made as layer tap.
Software was built with these changes and flashed central half.
But they didn't work. If the same mapping repeated with zmk studio it was working.

### Solution

Flash reset software (.uf2) file which gets generated along with left/right uf2.
Flashing should be done to right half then actual sw with proper keymaps.
Same step to be repeated for left half.

Just after flashing reset software, OS will shows connected device as SETTINGS RESET 
instead of "sofle"


Note: Same was happening with `backtick/~` mapped to top left in default layer.
After cleaning persistent storage with reset software, and then reflashing with new sw
it started working

