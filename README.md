# NGSwiftUIPreviewBuildPhaseIssue
Demonstrates an issue with automatic preview updating in SwiftUI. If you have a build script which edits a file in the project (e.g. build information you want available to the app, or code generation), SwiftUI previews will stop automatically updating.

To reproduce:

1. Clone the repo
2. Open the ContentView in Xcode with a preview
3. Change something
4. Click resume on the "Previews paused" banner

After the preview updates, the previews paused banner will reappear, and every subsequent time you want to update the preview, you have to build the whole app again.
