# lara-thumb
[![Total Downloads](https://poser.pugx.org/alex-kudrya/lara-thumb/downloads)](//packagist.org/packages/alex-kudrya/lara-thumb) [![Latest Unstable Version](https://poser.pugx.org/alex-kudrya/lara-thumb/v/unstable)](//packagist.org/packages/alex-kudrya/lara-thumb) 
[![License](https://poser.pugx.org/alex-kudrya/lara-thumb/license)](//packagist.org/packages/alex-kudrya/lara-thumb)

This script converts the original image into a thumbnail with the given sizes and various modes
Modes: 'cover', 'contain'.

## Example

```PHP

use kudrya/LaraThumb/LaraThumb

class MakeThumbnail()
{
  public function run(Request $request, int $width = 100, int $height = 100)
  {
    $file = $request->file('image');
    LaraThumb::processing($file, $width, $height, 'cover')
  }
};
```
