# SharpTest
A basic testing library for use with SFML.Net.

## Dependencies
- SFML.Net `https://github.com/graphnode/SFML.Net.git`

## Usage
If your test does not require visual output, your class should should inherit from `TestModule` and
testing should be done in `OnTest()`.<br>
If your test does require visual output, your class should inherit from `VisualTestModule`, do
non-visual testing in `OnTest()` and do visual testing in `OnVisualTest(RenderWindow)`.<br>
Once your tests are written, they can be ran with `Testing.Test<TestType>(RenderWindow)`, leaving
the render window null for non-visual tests.

## Changelog

### Version 0.1.0
- Initial release.
