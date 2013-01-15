## MBAlertView
===================

MBAlertView is a fun and simple block-based alert and HUD library for iOS.

### Features
<ul>
	<li>Nested alerts and HUDs</li>
	<li>Block based</li>
	<li>Images</li>
	<li>Nice animations</li>
	<li>Doesn't use any PNG files. Everything is drawn with code.</li>
</ul>

## Usage

There are two factory methods to get you started:

### Alerts

``` objective-c
MBAlertView *alert = [MBAlertView alertWithBody:@"Are you sure you want to delete this note? You cannot undo this." cancelTitle:@"Cancel" cancelBlock:nil];
   [alert addButtonWithText:@"Delete" type:MBAlertViewItemTypeDestructive block:^{ // delete }];
[alert addToDisplayQueue];
```

### HUDs
``` objective-c
[MBHUDView hudWithBody:@"Wait." type:MBAlertViewHUDTypeActivityIndicator hidesAfter:4.0 show:YES];
```

## License
MBAlertView is available under the MIT license.