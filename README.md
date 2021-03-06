#iOS-blur

In iOS 7 a new view is shown in several places that is transparent and has a blur on it. Sadly Apple hasn't given us a proper API to use a similar view.

Apple gave us some sample code at WWDC that can take an UIImage and add blur to it. It looks great, but isn't as cool as a view that adds blur to the views behind it in realtime.

So after 3 and a half cups of coffee I came up with a brilliant and simple idea. It does, however, only work for iOS 7.

> It seems Apple are rejecting Apps that use this code, so use with caution.
> Read more in this issue: 
> https://github.com/JagCesar/iOS-blur/issues/25
> - Note that I've changed the name of the class, seems Apple are simply looking for the class AMBlurView. The new class name is JCRBlurView

##Screenshot
![Screenshot](https://raw.github.com/JagCesar/iOS-blur/master/screenshot.png "Example of JCRBlurView")

##How is it done?

It's a real simple solution. I simply took a UIToolbar, placed it as a subview and voila!

##Awesome! So, how do I use it?

Simply copy the class JCRBlurView to your project, initialise it, set a frame and add it to your view. Voila!

```
JCRBlurView *blurView = [JCRBlurView new];
[blurView setFrame:CGRectMake(0.0f,0.0f,100.0f,100.0f)];
[self.view addSubview:blurView];
```

##License
iOS-blur is released under the WTFPL-license (see the LICENSE file)
