<div class="header-banner tropical">
     <div class="header-label tropical">Jump, Label & Return Event</div>
</div>

*The Jump event is used for changing the flow of the timeline and changing to another timeline. It's naturally tied to the Label event.
The jump flow is closely knit to the Label event and the Return event.*

## 📜 Content
[toc]


## 1. Text Syntax

Using `jump` without any target will set the next event to the beginning of this current timeline.

```dtl
# Using "jump" returns to the beginning of this timeline.
character: Hello, this is the start.
character: This is the second message.
jump
```

Let's introduce labels using the Label event. This will print `Hello 1`, `Hello 2`, and `Hello 3`. After this, the jump will print `Hello 2` and `Hello 3`.

```
dtl
character: Hello 1
label your_label_name
character: Hello 2
character: Hello 3
jump your_label_name
```

---

## 2. The Jump Stack
Whenever you use the Jump event, it will track where you are before changing the flow. This allows using the Return event, which reverses the flow back to the last jump point.
If you jump from timeline A to timeline B's start point and use the Return event in timeline B, it will revert to timeline A. This logic behaviour is implemented using a stack.

## 3. Jump Flow via Code

### 3.1 Starting at a Label
If you want to start at a specific label, you can provide this to your start event: `Dialogic.start(timeline, "your_label_name")`.

### 3.2 Jump Signals
Have a look at our signals here: [List of all signals](../classes/subsystem_jump.html#signals).

## 3.3 Jumping directly
If starting at a label is not enough, you can use `Dialogic.Jump.jump_to_label(label: String)` as well. This does not use the jump stack.
Alternatively, you can use `Dialogic.Jump.resume_from_last_jump()`.

