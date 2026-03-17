# async-keyboard-pointer

Use keyboard and pointer events asynchronously.

## Installation

npm i @dandre3000/async-keyboard-pointer

## Usage

## Exports

<h4>
    interface PointerState {<br/>
        button1: boolean<br/>
        button2: boolean<br/>
        button3: boolean<br/>
        button4: boolean<br/>
        button5: boolean<br/>
        screenX: number<br/>
        screenY: number<br/>
        clientX: number<br/>
        clientY: number<br/>
        pageX: number<br/>
        pageY: number<br/>
        movementX: number<br/>
        movementY: number<br/>
    }
</h4>

#### getPointerStates: (...idArray: [number]) => PointerState
#### getPointerStates: (...idArray: number[]) => PointerState[]

#### getPointerStateMap: () => Map<number, PointerState>

#### getKeyboardButtons: (...codeArray: [string]) => boolean
#### getKeyboardButtons: (...codeArray: string[]) => boolean[]

#### getKeyboardState: () => Set<string>

#### asyncPointerenter: (id: PointerEvent["pointerId"], signal?: AbortSignal) => Promise<PointerState>

#### asyncPointerdown: (id: PointerEvent["pointerId"], signal?: AbortSignal) => Promise<PointerState>

#### asyncPointermove: (id: PointerEvent["pointerId"], signal?: AbortSignal) => Promise<PointerState>

#### asyncPointerup: (id: PointerEvent["pointerId"], signal?: AbortSignal) => Promise<PointerState>

#### asyncClick: (id: PointerEvent["pointerId"], signal?: AbortSignal) => Promise<PointerState>

#### asyncPointerleave: (id: PointerEvent["pointerId"], signal?: AbortSignal) => Promise<PointerState>

#### asyncKeydown: (code: KeyboardEvent["code"], signal?: AbortSignal) => Promise<boolean>

#### asyncKeypress: (code: KeyboardEvent["code"], signal?: AbortSignal) => Promise<boolean>

#### asyncKeyup: (code: KeyboardEvent["code"], signal?: AbortSignal) => Promise<boolean>

## License

[MIT](https://github.com/dandre3000/async-keyboard-pointer/blob/main/LICENSE)
