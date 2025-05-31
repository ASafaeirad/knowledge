> Don't bake rigid rules into your system. Build flexible tools instead.

A system should provide flexible, general tools (mechanisms) rather than impose rigid rules or specific behaviors (policies) on how those tools must be used.

**In simple terms:**
> **Mechanism** = _“Here’s a way to do something.”_  
> **Policy** = _“Here’s the way you must do it.”_

## Example in software:
- Mechanism: A file system lets you set permissions on files (read/write/execute) — that's a mechanism.
- Policy: The system forces all files to be read-only — that’s a policy.

By choosing mechanism over policy, the system lets users decide how they want to use the tools provided, making it more flexible and adaptable to different needs.

### Why it matters:

**Flexibility**: Users can implement their own policies using the provided tools.

**Reusability**: The same mechanism can support many different use cases.

**Avoids assumptions**: It doesn’t assume what is "best" for every user or situation.

## Origin:

This idea comes from early Unix philosophy and is also echoed in books like The **Pragmatic Programmer**. It encourages designing systems that empower users and developers, rather than constrain them with fixed ideas about usage.
