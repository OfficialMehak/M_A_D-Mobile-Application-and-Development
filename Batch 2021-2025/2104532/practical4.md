
# Android User Interface Design: Practical 4

## 1. LinearLayout
- **Description**: Arranges its children in a single row or column.
- **Orientation**: `android:orientation="vertical"` for a vertical layout, `android:orientation="horizontal"` for a horizontal layout.

```xml
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"/>

    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Click Me"/>

</LinearLayout>
```

## 2. RelativeLayout
- **Description**: Positions its children relative to each other or the parent container.
- **Attributes**: `android:layout_alignParentTop`, `android:layout_below`, `android:layout_centerInParent`, etc.

```xml
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        android:layout_centerInParent="true"/>

    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Click Me"
        android:layout_below="@id/textView"
        android:layout_centerHorizontal="true"/>

</RelativeLayout>
```

## 3. GridLayout
- **Description**: Places its children in a grid (rows and columns).
- **Attributes**: `android:layout_row`, `android:layout_column`, `android:layout_rowSpan`, etc.

```xml
<GridLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:columnCount="2"
    android:rowCount="2">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Item 1"
        android:layout_row="0"
        android:layout_column="0"/>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Item 2"
        android:layout_row="0"
        android:layout_column="1"/>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Item 3"
        android:layout_row="1"
        android:layout_column="0"/>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Item 4"
        android:layout_row="1"
        android:layout_column="1"/>

</GridLayout>
```

## 4. TableLayout
- **Description**: Arranges its children in rows and columns similar to an HTML table.
- **Components**: `TableRow` is used to define rows.

```xml
<TableLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Item 1"/>

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Item 2"/>
    </TableRow>

    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Item 3"/>

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Item 4"/>
    </TableRow>

</TableLayout>
```
