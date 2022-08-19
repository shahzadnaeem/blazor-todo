# Notes

## VSCode Razor Language Server Crashes

```text
This is an OpenSSL 3 related issue and the fix is the following:

    export CLR_OPENSSL_VERSION_OVERRIDE=1.1
```

## .razor.css File Changes Don't 'Work'

[CSS Isolation](https://docs.microsoft.com/en-us/aspnet/core/blazor/components/css-isolation)

Hot reload does not deal with new `Component.razor.css` files.

Fix is to do a manual `dotnet build` 🤕 and then go back to `dotnet run watch`

## Learn Razor Syntax 😁

[Razor Syntax](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/razor)

Especially `Conditional Attributes` - or use `@( ?: )`
