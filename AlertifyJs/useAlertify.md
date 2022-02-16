## Alertify Js


```
 * @title {String or DOMElement} The dialog title.
 * @message {String or DOMElement} The dialog contents.
 * @onok {Function} Invoked when the user clicks OK button or closes the dialog.
 * alertify.alert(title, message, onok);
 
alertify.alert('Alert Title', 'Alert Message!', function(){ alertify.success('Ok'); });
```
set() is used to set properties values.

**Set Multiple Properties**

```
alertify.alert()
  .setting({})  // Object with properties and it's values
```

**Dialog should be closable**

```
 alertify.alert('Closable: true').set('closable', true); 
```

**When anyone clicks anywhere other than modal**

```
 alertify.alert('closableByDimmer: false').set({'closableByDimmer': false}); 
```

**Removes the frame of the dialog**

```
 alertify.alert('Frameless: true').set('frameless', true); 
 ```
 
 **Invoke something when user clicks close**
 
 ```
 alertify.alert('invokeOnCloseOff: false')
         .set({'invokeOnCloseOff': false,'onok': function(){alertify.success('Ok')} });
  ```
 
 **Change Label**
 
 ```
  alertify.alert('label changed!').set('Initial', 'Final'); 
 ```
 
 **Make Dialog Resizable**
 
 ```
  alertify.alert('Maximizable: true').set('maximizable', true);  // Boolean Value
 ```
 
 **Set Content of Dialog**
 
 ```
  alertify.alert().set('message', 'This is a new message!')
 ```
 
 **Modal restricts surfing website also if it is open**
 
 ```
  alertify.alert('Modal: true').set('modal', true);   // Use false for not restrict
 ```
 
 **User can move modal**
 
 ```
  alertify.alert('Movable: false').set('movable', true);  // Boolean Value
 ```
 
**Manage Content Overflow**

```
 alertify.alert().set('overflow',true); // Boolean Value
```

**Manage Padding**

```
 alertify.alert().set('padding',true);  // Boolean Value

```
**Modal can be pinned**

```
 alertify.alert('Content').set({'pinnable',true}); // Boolean Value
```

**Dialog is Resizable**

```
 alertify.alert('Resizable: true').set('resizable', true); 
```

**Set Transition effect**

```
 alertify.alert().set({transition:'pulse',message: 'pulse'})
```

- slide
- Zoom
- pulse
- flipx
- flipy
- fade

**Remove effect of transition**

```
 alertify.alert().set({transitionOff:true,message: 'Transition Off'}) 
```

**EVENTS AVAILABLE**

-  onclose
-  onclosing
-  onfocus
-  onmaximize
-  onmaximized
-  onmove
-  onmoved
-  onok
-  onresize
-  onresized
-  onrestore
-  onrestored

we can use `set({eventName:function(){}})`



