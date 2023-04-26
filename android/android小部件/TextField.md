
```kotlin

public fun TextField(
    value: String, // 和下面的onValueChange结合，设置为可变状态之后，文本框才能正常输入。
    onValueChange: (String) -> Unit, // { 可变状态 = it }
    modifier: Modifier,
    enabled: Boolean,
    readOnly: Boolean,
    textStyle: TextStyle,
    label: @Composable() (() -> Unit)?,  // {标签} 打上大括号之后不容易出错。
    placeholder: @Composable() (() -> Unit)?,  // 在键入函数时最好是打上大括号，这样不容易出错。
    leadingIcon: @Composable() (() -> Unit)?,
    trailingIcon: @Composable() (() -> Unit)?,
    supportingText: @Composable() (() -> Unit)?,
    isError: Boolean,
    visualTransformation: VisualTransformation,
    keyboardOptions: KeyboardOptions, // 键盘选项：可以把键盘设置成弹出数字键盘或者其他。
    keyboardActions: KeyboardActions,
    singleLine: Boolean,   // 是否单行模式
    maxLines: Int,
    interactionSource: MutableInteractionSource,
    shape: Shape,
    colors: TextFieldColors
): Unit
