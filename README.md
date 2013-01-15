 MBAlertView
===================

MBAlertView is a fun and simple block-based alert and HUD library for iOS, as seen in [Notestand.](https://itunes.apple.com/us/app/notestand-notes-discussions/id586976282?mt=8)

<img src="http://i.imgur.com/3s3eJ.png" alt="alert1" title="alert1" style="margin-right:10px; margin-left:10px; float:left;">

<img src="http://i.imgur.com/7CbbT.png" alt="hud1" title="hud1" style="display:block;margin-right:10px; float:left;">

<img src="http://i.imgur.com/lq53u.png" alt="hud2" title="hud2" style="display:block; margin-right:10px;  float:left;">

<img src="http://i.imgur.com/Aqfnr.png" alt="hud2" title="hud2" style="display:block; margin-right:10px;">

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

You can see more in the easy to follow demo.

## License
MBAlertView is available under the MIT license.