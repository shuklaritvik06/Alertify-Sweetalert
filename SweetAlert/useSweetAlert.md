## SweetAlert

There are four icons: "warning", "error", "success" and "info".

```swal(
title: "Title",
message: "Message",
icon: "Icon type",  // Can also be a URL
button: "Confirm button text",
buttons: true,
dangerMode: true,
timer: 2000,
closeOnEsc: false,
closeOnClickOutside: false,
content: {
element: "input",  // or slider
attributes: {
  placeholder: "Type your password",
  type: "password",
},

)
```

`swal.close()` => method To close the alert

Sweetalert use promises to handle user interaction. 

```swal("Click on either the button or outside the modal.")
.then((value) => {
  swal(`The returned value is: ${value}`);
});

```

**Multiple Buttons**

```
buttons: ["Oh no!", "COOl!"],

```

If we want one of the buttons to just have their default text, we can set the value to true instead of a string.

```
swal("Text", {
  buttons: {
    cancel: "No",
    OK: {
      text: "Yes!",
      value: "catch",
    },
    ignore: true,
  },
})
.then((value) => {
  switch (value) {
 
    case "ignore":
      swal("Ignored safely!");
      break;
 
    case "OK":
      swal("Got it","Completed Safely", "success");
      break;
 
    default:
      swal("Kuch choose to karo");
  }
});
```
**Buttons Options**

```
    text: "Cancel",
    value: null,
    visible: false,
    className: "",
    closeModal: true,
```

Class can also be added to the modal to give extra styling

```
  swal("Text", {
    className: "name",
  });
```

- swal overlay -> For styling the area around modal
- swal modal -> to style modal
- swal footer -> to style footer
- swal title -> to style title
- swal text -> to style text

**Ajax Req Example**

```



```

