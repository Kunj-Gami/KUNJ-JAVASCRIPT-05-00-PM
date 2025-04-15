# Element Methods and Properties Reference

| Category        | Element Type(s) | Method / Property         | Description                                                                 | Example Use Case                                    |
|-----------------|-----------------|--------------------------|-----------------------------------------------------------------------------|-----------------------------------------------------|
| **Input**       | Input Elements  | `.focus()`                | Sets focus on the element.                                                   | `ref.current.focus()`                               |
|                 |                 | `.blur()`                 | Removes focus from the element.                                                |                                                     |
|                 |                 | `.select()`               | Selects the text inside the input box.                                        |                                                     |
|                 |                 | `.value`                  | Reads/updates the value of the input.                                         |                                                     |
|                 |                 | `.disabled`               | Disables/enables the input.                                                    |                                                     |
| **Media**       | Audio/Video     | `.play()`                 | Plays the video/audio.                                                       | `ref.current.play()`                                |
|                 |                 | `.pause()`                | Pauses the playback.                                                          | `ref.current.pause()`                               |
|                 |                 | `.currentTime`           | Reads/sets the current time.                                                 |                                                     |
|                 |                 | `.volume`                 | Sets the volume.                                                              |                                                     |
|                 |                 | `.muted`                  | Mutes/unmutes the audio/video.                                                 |                                                     |
| **General**     | All Elements    | `.scrollIntoView()`       | Scrolls the element into view.                                                 | `ref.current.scrollIntoView()`                      |
|                 |                 | `.innerHTML`              | Sets/reads the HTML content.                                                   |                                                     |
|                 |                 | `.textContent`            | Sets/reads the text content.                                                   |                                                     |
|                 |                 | `.style`                  | Used to set inline styles.                                                     | `ref.current.style.background = "red"`              ||                 |                 | `.classList.add()`        | Adds a class to the element.                                                  | `ref.current.classList.add("xyz")`                  |
|                 |                 | `.classList.remove()`     | Removes a class from the element.                                               |                                                     |
|                 |                 | `.classList.toggle()`     | Toggles the class on the element.                                               |                                                     |
|                 |                 | `.getBoundingClientRect()` | Provides the size and position of the element.                                |                                                     |
| **Scroll**      | All Elements    | `.scrollTop`              | Sets the vertical scroll position.                                            | `ref.current.scrollTop`                             |
|                 |                 | `.scrollLeft`             | Sets the horizontal scroll position.                                           |                                                     |
|                 |                 | `.offsetTop`              | Gets the element's top position (relative to parent).                           |                                                     |
|                 |                 | `.offsetHeight`           | Gets the height of the element.                                                 | `ref.current.offsetHeight`                          |
