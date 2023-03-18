We've been building apps for far too long to be bothered with convincing you that we know what we're doing and that you should listen to us. Do it or don't. Don't care.

If you want to build robust, scalable, performant apps for Android, iOS, Linux, macOS, Web, and Windows AND have a laugh while you're at it, then use geezer. Or don't. Don't care.

## get off my lawn

There's one code file format in geezer, just one, and it's `.goml`. Yup, that's short for "get off my lawn" and it looks like this:

```csharp
Page
    .Title("The Front Porch")
    .Content {
        Label
            .Text(@say)
        Button
            .Tap(@yell)
    }
```

## you'll poke your eye out

State management is a pita for any app, so let's make it dead simple. All state is immutable, which is fancy talk for you can't change it willy nilly and think you're app is gonna be just fine. Nope. 

When you need to update state, say if somebody actually decides to use your silly little app, then you send the value to the update method and a new state is created triggering the UI to render only the bit that changed. It's super fast. Don't be clever, just call update state.

```csharp
Page
    .Title("The Front Porch")
    .Content {
        Label
            .Text(@say)
        Button
            .Tap(@yell)
    }

Model = {
            say = "What a beautiful morning"
        }

yell()
{
    Model.say = "Get off my lawn!"
    Update()
}
```

## how's this thing work?

Oh, you want documentation? Get bent. Just start typing, and follow the code. Back in my day there was never any documentation, and you just learned to view source.

## stop whining and start coding

Ready to roll? Here's your installation:

```console
brew install geezer
```

Then create a new app:

```console
geezer get-bent MillionDollarsAndAJet
```

Ready to run?

```console
cd ./MillionDollarsAndAJet
geezer giddyup
```

Bam, you've got an app! Ya happy now?! Kids these days...