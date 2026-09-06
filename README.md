# Horion Injector (fork)

This fork preserves the original Horion injector while making source-built use a little safer and easier to understand.

## Build

1. Install Visual Studio with **.NET desktop development**.
2. Open `HorionInjector.sln`.
3. Select `Release | x64`.
4. Build the solution.

The project targets **.NET Framework 4.8** and **x64**.

## Important security note

The original injector can download `Horion.dll` from `https://horion.download`. That DLL is a separate binary from this repository, so building this injector from source does **not** verify the contents of the downloaded DLL.

If source transparency matters, prefer using a DLL that you built yourself and review or scan any downloaded DLL before loading it.

## Controls

- **Left click Inject:** downloads the current Horion DLL from the configured Horion server, then injects it.
- **Right click Inject:** lets you select a local DLL.

This project is intended for Minecraft Bedrock modding. Use it only on systems and game environments where you have permission to do so.
