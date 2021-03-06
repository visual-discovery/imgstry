[imgstry](../README.md) › [Globals](../globals.md) › [ImgstryEditor](imgstryeditor.md)

# Class: ImgstryEditor

Defines the imgstry editor schema.

**`export`** 

**`interface`** ImgstryEditor

**`template`** 

## Hierarchy

* ImgstryProcessor

  ↳ **ImgstryEditor**

  ↳ [Imgstry](imgstry.md)

  ↳ [Imgstry](imgstry.md)

## Index

### Properties

* [height](imgstryeditor.md#abstract-height)
* [width](imgstryeditor.md#abstract-width)

### Accessors

* [histogram](imgstryeditor.md#histogram)
* [imageData](imgstryeditor.md#imagedata)

### Methods

* [batch](imgstryeditor.md#batch)
* [blackAndWhite](imgstryeditor.md#blackandwhite)
* [brightness](imgstryeditor.md#brightness)
* [clear](imgstryeditor.md#clear)
* [clone](imgstryeditor.md#abstract-clone)
* [contrast](imgstryeditor.md#contrast)
* [convolve](imgstryeditor.md#convolve)
* [createImageData](imgstryeditor.md#abstract-createimagedata)
* [fill](imgstryeditor.md#fill)
* [gamma](imgstryeditor.md#gamma)
* [hue](imgstryeditor.md#hue)
* [invert](imgstryeditor.md#invert)
* [noise](imgstryeditor.md#noise)
* [render](imgstryeditor.md#abstract-render)
* [renderSync](imgstryeditor.md#rendersync)
* [reset](imgstryeditor.md#abstract-reset)
* [saturation](imgstryeditor.md#saturation)
* [sepia](imgstryeditor.md#sepia)
* [tint](imgstryeditor.md#tint)
* [toDataUrl](imgstryeditor.md#abstract-todataurl)
* [vibrance](imgstryeditor.md#vibrance)

## Properties

### `Abstract` height

• **height**: *number*

*Inherited from void*

*Defined in [core/imgstry.processor.ts:36](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.processor.ts#L36)*

Height of the image.

**`memberof`** ImgstryProcessor

___

### `Abstract` width

• **width**: *number*

*Inherited from void*

*Defined in [core/imgstry.processor.ts:29](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.processor.ts#L29)*

Width of the image.

**`memberof`** ImgstryProcessor

## Accessors

###  histogram

• **get histogram**(): *HistogramData*

*Inherited from void*

*Defined in [core/imgstry.processor.ts:106](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.processor.ts#L106)*

Returns the channel histogram of the image.

**`readonly`** 

**`memberof`** ImgstryProcessor

**Returns:** *HistogramData*

___

###  imageData

• **get imageData**(): *ImageData*

*Inherited from void*

*Defined in [core/imgstry.processor.ts:89](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.processor.ts#L89)*

Gets the image data.

**`abstract`** 

**`memberof`** ImgstryProcessor

**Returns:** *ImageData*

• **set imageData**(`imgData`: ImageData): *any*

*Inherited from void*

*Defined in [core/imgstry.processor.ts:97](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.processor.ts#L97)*

Sets the image data.

**`abstract`** 

**`memberof`** ImgstryProcessor

**Parameters:**

Name | Type |
------ | ------ |
`imgData` | ImageData |

**Returns:** *any*

## Methods

###  batch

▸ **batch**(`options`: OperationOption[], `reset?`: undefined | false | true): *ImgstryProcessor*

*Inherited from void*

*Defined in [core/imgstry.processor.ts:136](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.processor.ts#L136)*

Applies a series of filters to the image.

**`memberof`** ImgstryProcessor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`options` | OperationOption[] | The set of operations. |
`reset?` | undefined &#124; false &#124; true | - |

**Returns:** *ImgstryProcessor*

The current processor instance

___

###  blackAndWhite

▸ **blackAndWhite**(`ratio?`: [number, number, number]): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:28](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L28)*

Turn the image black and white with the provided ratio.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type |
------ | ------ |
`ratio?` | [number, number, number] |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

###  brightness

▸ **brightness**(`value`: number): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:50](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L50)*

Increase / decrease image brightness.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`value` | number | brightness intensity |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

###  clear

▸ **clear**(): *this*

*Defined in [core/imgstry.editor.ts:169](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L169)*

Clears the operation list.

**`memberof`** ImgstryEditor

**Returns:** *this*

the current editor instance

___

### `Abstract` clone

▸ **clone**(`source`: ImageData): *ImageData*

*Inherited from void*

*Defined in [core/imgstry.processor.ts:72](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.processor.ts#L72)*

Clone image data

**`abstract`** 

**`memberof`** ImgstryProcessor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`source` | ImageData | The source image data. |

**Returns:** *ImageData*

The cloned canvas image data.

___

###  contrast

▸ **contrast**(`value`: number): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:39](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L39)*

Increase / decrease image constrast.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`value` | number | contrast intensity |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

###  convolve

▸ **convolve**(`kernel`: [Kernel](kernel.md) | number[][]): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:159](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L159)*

Apply a kernel to the active image

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`kernel` | [Kernel](kernel.md) &#124; number[][] | a square matrice that will be applied to the image |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

### `Abstract` createImageData

▸ **createImageData**(`source`: ImageData): *ImageData*

*Inherited from void*

*Defined in [core/imgstry.processor.ts:81](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.processor.ts#L81)*

Create image data based on a source

**`abstract`** 

**`memberof`** ImgstryProcessor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`source` | ImageData | The source image data. |

**Returns:** *ImageData*

The new image data.

___

###  fill

▸ **fill**(`color`: string): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:148](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L148)*

Fill the canvas with a color.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`color` | string | the hex color code of the desired tint |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

###  gamma

▸ **gamma**(`value`: number): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:94](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L94)*

Increase / decrease image gamma.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`value` | number | gamma intensity |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

###  hue

▸ **hue**(`value`: number): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:72](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L72)*

Shift the image hue.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`value` | number | hue shift value (-180, 180) |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

###  invert

▸ **invert**(): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:126](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L126)*

Invert the image colors.

**`memberof`** ImgstryEditor

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

###  noise

▸ **noise**(`value`: number): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:105](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L105)*

Add a provided amount of noise to the image.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`value` | number | noise amount |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

### `Abstract` render

▸ **render**(`target`: RenderTarget): *Promise‹[ImgstryEditor](imgstryeditor.md)›*

*Defined in [core/imgstry.editor.ts:193](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L193)*

Apply the requested operations to the image using a worker thread.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`target` | RenderTarget | the processing target |

**Returns:** *Promise‹[ImgstryEditor](imgstryeditor.md)›*

a promise that resolves in the current editor instance

___

###  renderSync

▸ **renderSync**(`target`: RenderTarget): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:181](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L181)*

Apply the requested operations to the image.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`target` | RenderTarget | "current" | the processing target |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

### `Abstract` reset

▸ **reset**(): *ImgstryProcessor*

*Inherited from void*

*Defined in [core/imgstry.processor.ts:63](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.processor.ts#L63)*

Resets the image to the original state.

**`abstract`** 

**`memberof`** ImgstryProcessor

**Returns:** *ImgstryProcessor*

The current processor instance.

___

###  saturation

▸ **saturation**(`value`: number): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:61](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L61)*

Increase / decrease image saturation.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`value` | number | saturation intensity |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

###  sepia

▸ **sepia**(`value`: number): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:83](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L83)*

Apply sepia with the specified intensity.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`value` | number | desired intensity of the sepia effect |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

###  tint

▸ **tint**(`color`: string): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:137](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L137)*

Apply a color tint to the image.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`color` | string | the hex color code of the desired tint |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance

___

### `Abstract` toDataUrl

▸ **toDataUrl**(`type`: string): *string*

*Inherited from void*

*Defined in [core/imgstry.processor.ts:53](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.processor.ts#L53)*

Encodes the canvas data to a data URI.

**`memberof`** Imgstry

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`type` | string | The standard MIME type for the image format to return. If you do not specify this parameter, the default value is a PNG format image. |

**Returns:** *string*

The image encoded as a data url.

___

###  vibrance

▸ **vibrance**(`value`: number): *[ImgstryEditor](imgstryeditor.md)*

*Defined in [core/imgstry.editor.ts:116](https://github.com/visual-cortex/imgstry/blob/master/source/core/imgstry.editor.ts#L116)*

Increase / decrease image vibrance.

**`memberof`** ImgstryEditor

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`value` | number | vibrance intensity |

**Returns:** *[ImgstryEditor](imgstryeditor.md)*

the current editor instance
