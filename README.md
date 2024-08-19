![alt text](https://i.ibb.co/nb1cpGT/sye-banner.png?raw=true)
# Biometric Authentication Plugin for Unity
![alt text](https://i.ibb.co/56f4d7N/cover-image.png?raw=true)
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
- For a complete example, import the sample from the Package Manager and refer to the demo scene. This scene provides a full implementation that you can build for all supported platforms.
- **Example Video**: [Watch on YouTube](https://youtu.be/LNZqCBFtb0g)

## Notes for Each Platform
- **iOS/macOS**: Works out-of-the-box with Face ID and Touch ID.
- **Android**: Automatically sets up Android BiometricPrompt.
- **WebGL**: Supports biometrics depending on browser capabilities.

## Troubleshooting
- **Build Errors**: Check that your Unity project targets supported platforms.
- **Authentication Fails**: Make sure biometrics are set up on the test device.
- **Android Issues**: Check for conflicts in the `AndroidManifest.xml` if using other plugins.

## Links
- **Asset Store Package**: [Biometrics Authentication Plugin](https://assetstore.unity.com/packages/slug/293752)
- **Example Video**: [Watch on YouTube](https://youtu.be/LNZqCBFtb0g)

## Version
- **1.0.0**: Initial release.

## License

This plugin is licensed under [Standard Unity Asset Store EULA](https://unity.com/legal/as-terms).

## Contact

For any questions or support, feel free to reach out at [aqaddora96@gmail.com](mailto:aqaddora96@gmail.com).

---

Thank you for using the `Biometrics Authentication` plugin! We hope it simplifies the process of integrating biometrics authentication into your Unity projects.
