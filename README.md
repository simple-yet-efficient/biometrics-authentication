# Biometric Authentication Plugin for Unity

## Overview
This plugin lets you add biometric authentication (like Face ID or Android Biometrics) to your Unity projects. It supports iOS, macOS, Android, and WebGL.

## Supported Platforms
- **iOS**
- **macOS**
- **Android**
- **WebGL**

## How to Use

1. **Call `Authenticate` Method**:
   - Simply call the `SyE.BiometricsAuthentication.Biometrics.Authenticate` method in your script, passing in the `onSuccess` and `onFailure` callbacks.

```csharp
using SyE.BiometricsAuthentication;

public class YourScript : MonoBehaviour
{
    void Start()
    {
        Biometrics.Authenticate(
            onSuccess: () => Debug.Log("Authenticated successfully"),
            onFailure: () => Debug.LogError("Authentication failed")
        );
    }
}
```

## Example
- For a complete example, refer to the demo scene included with the plugin. This scene provides a full implementation that you can build for all supported platforms.

## Notes for Each Platform
- **iOS/macOS**: Works out-of-the-box with Face ID and Touch ID.
- **Android**: Automatically sets up Android BiometricPrompt.
- **WebGL**: Supports biometrics depending on browser capabilities.

## Troubleshooting
- **Build Errors**: Check that your Unity project targets supported platforms.
- **Authentication Fails**: Make sure biometrics are set up on the test device.
- **Android Issues**: Check for conflicts in the `AndroidManifest.xml` if using other plugins.

## Version
- **1.0.0**: Initial release.
