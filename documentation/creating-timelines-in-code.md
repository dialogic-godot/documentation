<div class="header-banner blurple">
     <div class="header-label blurple">Creating Timelines in Code</div>
</div>

*As timelines and events are just resources, you can create new timelines in code.*

## 📜 Content
[toc]

# How do I create timelines via code?

Creating an empty timeline would look like this:

```gdscript
var timeline : DialogicTimeline = DialogicTimeline.new()
Dialogic.start_timeline(timeline)
```

Of course, the timeline created here doesn't contain events yet. To add events, you can do two things:

- Create an array of **event resources**:

  ```gdscript
  var events : Array = []
  var text_event = DialogicTextEvent.new()
  text_event.text = "Hey, this was made in code!"
  text_event.character = load("res://characters/Emilio.dch")
  events.append(text_event)

  var timeline : DialogicTimeline = DialogicTimeline.new()
  timeline.events = events
  # if your events are already resources, you need to add this:
  timeline.events_processed = true
  Dialogic.start(timeline)
  ```

- Create an array of **String**s:

  ```gdscript
  var events : Array = """
  Jowan (Surprised): Wow this is interesting!
  - Yes
      [background path="res://icon.png"]
      [wait seconds="1"]
      set MyAutoload.exitement += 20
  - No
      set MyAutload.exitement -= 10 """.split('\n')

  var timeline : DialogicTimeline = DialogicTimeline.new()
  timeline.events = events
  Dialogic.start(timeline)
  ```

  *In this case, you have to follow the syntax explained in [this tutorial](timeline-text-syntax.md).*
