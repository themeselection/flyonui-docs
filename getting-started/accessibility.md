# Accessibility

Learn how FlyonUI’s built-in accessibility features support inclusive web development with Tailwind CSS components.

> **Info:** FlyonUI is built on top of <a href="https://preline.co/plugins.html" class="link font-semibold link-primary" target="_blank">Preline’s</a> headless, unstyled Tailwind plugins, offering accessible and responsive UI components.

<!-------------------- Accessibility in FlyonUI -------------------->

{{< headsingle addClass="!mt-px" level="2" >}} Accessibility in FlyonUI {{< /headsingle >}}

Every component is designed to be inclusive, with built-in accessibility features that ensure a seamless experience for users of all abilities.

<!-------------------- Accessibility Manager -------------------->

## Accessibility Manager

FlyonUI includes an `HSAccessibilityObserver`, a centralized system that manages accessibility interactions across your UI. It enhances keyboard support, interaction consistency, and accessibility behavior with minimal configuration.

- **Keyboard Navigation:** Supports navigation via keys like Arrow, Enter, Space, Escape, Home, End, and Tab.
- **Focus Management:** Automatically handles focus between nested or overlapping interactive components.
- **Interaction Conflict Prevention:** Coordinates global events to avoid clashes between components.
- **Context Awareness:** Adapts to complex structures, such as dropdowns within modals.
- **Plug-and-Play Setup:** Components auto-register for accessibility handling—no manual configuration needed.
- **Optimized Performance:** Uses event delegation and efficient tracking for low overhead.
- **WCAG-Aligned Patterns:** Implements common accessibility practices out of the box.
- **First-Letter Navigation:** Quickly select items by typing the first letter in dropdowns or select menus.
- **State Tracking:** Maintains consistent state awareness (open/close) across components.
- **Modifier Key Awareness:** Understands keys like Ctrl, Shift, Alt, and Meta for robust keyboard control.

<!-------------------- WCAG compliance -------------------->

## WCAG Compliance

FlyonUI components are built with accessibility best practices in mind, including:

- Semantic markup and utility-first classes
- Sufficient color contrast
- Meaningful ARIA attributes
- Screen reader testing

> Note: While FlyonUI provides accessible defaults, achieving full WCAG compliance also depends on your implementation. Be sure to test components in your specific context.

<!-------------------- Open source & customizable -------------------->

## Open Source & Customizable

FlyonUI is completely open source and free to use. You’re encouraged to explore, extend, and tailor components to meet your unique accessibility requirements.
