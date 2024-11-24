# quickmath.nvim

Neovim plugin for doing quick math.

## Installation

Using [lazy.nvim](https://lazy.folke.io/):

```lua
{
  'tobias-walle/quickmath.nvim',
  cmd = { 'QuickMath' }
}
```

## Usage

The `QuickMath` command allows you to perform quick mathematical calculations directly within Neovim.

### Basic Usage

1. **Evaluate a Range of Lines:**

   You can select a range of lines in visual mode and then execute the `QuickMath` command to evaluate the mathematical expression contained within those lines.

   ```vim
   :'<,'>QuickMath
   ```

   This will open a new buffer displaying the result of the evaluated expression.

2. **Evaluate a Single Expression:**

   You can also pass a mathematical expression directly to the `QuickMath` command.

   ```vim
   :QuickMath 3 + 4 * (2 - 1)
   ```

   This will open a new buffer displaying the result of the expression `3 + 4 * (2 - 1)`.

### Interactive Buffer

When the result buffer is opened, you can modify the expression directly in the buffer.

The result will update live as you make changes.

- **Close the Result Buffer:**

  You can close the result buffer by pressing `q` or by leaving the buffer.

### Example Expressions

- Simple arithmetic: `:QuickMath 5 + 10`
- Using parentheses: `:QuickMath (8 + 2) * 3`
- Division and multiplication: `:QuickMath 20 / 4 * 2`

These examples demonstrate how you can quickly perform calculations without leaving your Neovim environment.
