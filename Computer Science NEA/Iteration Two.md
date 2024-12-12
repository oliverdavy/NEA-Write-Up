%%
#Development
%%
# Iteration Two

The goal of this iteration was to set up a GUI using the designs from earlier. This UI will not have any functionality implemented at this point.  

First, the default greeting composable was removed.  

Then made a title bar using a surface to add colour and a text to add the title. Modifiers were then used to add adequate padding around the title and have it fill the whole screen width

```kotlin
@Composable
fun MyTopBar(title: String, modifier: Modifier = Modifier){
	Surface(
		color = Material.colorScheme.primaryContainer,
		modifier = Modifier.fillMaxWidth()
	){
		Text(
			text = title,
			fontSize = 40.sp,
			color = MaterialTheme.colorScheme.primary,
			modifier = modifier.padding(10.dp)
		)
	}
}
```
>Top Bar Title

Then added an icon button using the material UI icons to add a menu button. 

Put this in a row with the title.

```kotlin
Row { 
    IconButton( 
        onClick = {/* TODO */ }, 
        modifier = Modifier.padding(10.dp) 
    ) { 
        Icon( 
            imageVector = Icons.Rounded.Menu, 
            contentDescription = "Menu Icon", 
            modifier.size(40.dp) 
        ) 
    } 
 
    Text( 
        text = title, 
        fontSize = 40.sp, 
        color = MaterialTheme.colorScheme.primary, 
        modifier = Modifier.padding(10.dp) 
    ) 
} 
```

Then created a preview so the final top bar could be viewed without building the whole app.

```kotlin
@Preview 
@Composable 
fun TopBarPreview(){ 
    NEAProgrammingProjectTheme { 
        MyTopBar(title = "Metronome") 
    } 
} 
```

This gave this final preview

(top bar preview image)

This was then committed to the Git repository with the note "Top bar added"

Then added BPM display and a preview for that

```kotlin
@Composable 
fun BPMDisplay(currentBPM: String, modifier: Modifier = Modifier){ 
    Text( 
        text = currentBPM, 
        fontSize = 50.sp, 
        color = MaterialTheme.colorScheme.primary, 
        modifier = Modifier.padding(10.dp) 
    ) 
} 
```
>BPM Display

