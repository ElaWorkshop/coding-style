# Ela Coding Style

## Commit Messages

### Complete

Use sentence case. Use simple present tense. If the commit is issue related, add a prefix “[Verb #ID] ” (don’t forget the trailing space). Available verbs are **Fix**, **Close**, and **On** (**Fix** and **Close** will close the issue).

**For example:**
```
[Fix #3] Migrate to AFNetworking 2.0
```

```
[On #2] Try TEAChart
```

**But not:**
```
[Fix #3] Migrated to AFNetworking 2.0
```

```
migrated to afn 2.0
```

```
trying TEAChart
```

### Explicit

Use explicit description.

**For example:**
```
Fix table view cell text overflow
```

**But not:**
```
bug fix
```

### Write a Body If It’s Too Long

**For example:**
```
Fix a bug where 3D Touch shortcuts could generate invalid taiyakies

If Expense was launched by 3D Touch shortcut, `viewDidLoad` would be called after `prepareForSegue:sender:`. Some of the properties would not be initialized.
```

**But not:**
```
Fix a bug where 3D Touch shortcuts could generate invalid taiyakies because some of the properties would not be initialized
```

### Use Emoji

**For example:**
```
Release 1.0 🍻
```

**But not:**
```
Release 1.0
```

## Objective-C Style

Follow [NYTimes Style Guide](https://github.com/NYTimes/objective-c-style-guide).

Except that we write method implementation’s beginning bracket in a single line, as:

```objc
- (IBAction)dateChanged:(UIDatePicker *)sender
{
    self.dateField.text = [sender.date dateString];
}
```

One thing to emphasize, DO NOT use any abbreviations unless they are very common. Long variable names are not bad.
