# Accessibility

## Commitment

The GitHub Annotation Toolkit aims to support disabled designers, engineers,
and other collaborators in creating, reading, and discussing annotations. This
statement covers the Figma library and its documentation, rather than the
accessibility of products that use its annotations.

### Figma

Figma [documents keyboard and screen-reader support for canvas objects](https://www.figma.com/blog/introducing-screenreader-and-accessibility-features/).
Its [accessibility guidance](https://help.figma.com/hc/en-us/articles/35063862380311-Accessibility-at-Figma)
covers navigation, screen-reader settings, canvas zoom, interface scaling, and
enhanced interface contrast.

Canvas zoom enlarges annotations, while interface scaling enlarges Figma's
controls. Enhanced interface contrast changes Figma's interface, not the
library's stamp colors.

### Library design

Stamps mark design elements. Details components hold accompanying written
explanations.

- Text labels and icons distinguish annotation types without relying on color
  alone.
- The palette pairs stamp labels with contrasting backgrounds. Outlines and
  shadows help separate stamps from the canvas and the designs they overlap.
- Pin, Bracket, and Lasso formats offer different ways to point to an element
  or group. Adjustable label positions help keep the underlying design visible.
- Matching note numbers connect Stamps and Details visually. Optional fields
  let authors adjust the amount of detail without crowding the design.

The [Getting started guide](./basics/getting-started.md) explains these options.

### Documentation

[Tutorials and checklists](./README.md#tutorials-training-and-documentation)
provide written guidance outside Figma. They explain how to use annotations
and what information to capture; they do not reproduce the content of each
annotated design.

## Report an accessibility issue

Report barriers through the [public issue tracker](https://github.com/github/annotation-toolkit/issues).
Include the affected component or documentation page, the task, and a written
explanation of what blocks or complicates it.

Screenshots, recordings, and details about Figma, the browser, operating system,
or assistive technology are optional. Do not include confidential designs or
medical information in public reports.

## Known barriers

### Visual relationships on the canvas

Stamps and Details rely on canvas position, connecting lines, and matching note
numbers to communicate relationships. Access to an individual canvas object is
not equivalent to understanding which element an annotation describes or how
it relates to other notes.

These are library components, not Figma's native annotations. Accessibility
features for native annotations or prototypes do not automatically apply to
those relationships.

For collaborators who cannot follow the canvas, provide a structured text
description alongside the design. Identify the element, its intended semantics
and behavior, and any relevant ordering. Agree on a format that collaborators
can use; a walkthrough can supplement that written record.

### Dense or overlapping annotations

Complex designs with many annotations are difficult to follow when stamps
overlap, obscure content, or sit far from their Details. The
[best practices for annotating](./deep-dives/best-practices-for-annotating.md)
describe ways to reduce clutter by moving labels outside the design, keeping
Details in the margins, and separating complex annotations across frames.

Outlines and shadows do not guarantee legibility on every background. Review
contrast and readability in context, especially after changing colors, effects,
or placement.

## Testing

The [contribution process](./CONTRIBUTING.md) includes maintainer review and
testing of library changes before merge and publication. The project has not
conducted keyboard-only or screen-reader testing of this library, and the
repository does not run automated accessibility checks.

This statement describes design choices, not measured contrast ratios or a
claim of conformance with the Web Content Accessibility Guidelines (WCAG).

Annotations describe intended semantics and interactions; they do not implement
them in Figma or production code. Products built from annotated designs need
their own accessibility evaluation. [Annotation theory](./deep-dives/annotation-theory.md)
explains the role of annotations as a communication tool.

## Contributing

The [contribution guide](./CONTRIBUTING.md) explains how to propose library
changes. This project accepts direct Figma library contributions from GitHub
staff; other contributors can share suggestions and examples through issues.

For accessibility-related changes, describe the barrier or access need and
distinguish observed behavior from assumptions. Documentation improvements can
include clearer instructions, descriptive links, and text alternatives for
illustrations.

## Contact

GitHub's Accessibility Design team [maintains the toolkit](./README.md#maintainers).
[Support guidance](./SUPPORT.md) lists the public feedback route and additional
channels for GitHub staff.
