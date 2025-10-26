<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
	<key>IDECodeSnippetCompletionPrefix</key>
	<string>add observer UI thread</string>
	<key>IDECodeSnippetCompletionScopes</key>
	<array>
		<string>ClassImplementation</string>
	</array>
	<key>IDECodeSnippetContents</key>
	<string>        __weak typeof(self) weakself = self;
        [[NSNotificationCenter defaultCenter] addObserverForName:HRSMyHRSUserLoggedInUserDidChangeNotification object:nil queue:[NSOperationQueue mainQueue] usingBlock:^(NSNotification *note) {
            typeof(weakself) self = weakself;
            if (self == nil) {
                return;
            }
            [self myHRSLoggedInUserDidChange:note];
        }];
</string>
	<key>IDECodeSnippetIdentifier</key>
	<string>11D55EBF-9BBB-4B96-A14F-6A093FA5C171</string>
	<key>IDECodeSnippetLanguage</key>
	<string>Xcode.SourceCodeLanguage.Objective-C</string>
	<key>IDECodeSnippetTitle</key>
	<string>add observer UI thread</string>
	<key>IDECodeSnippetUserSnippet</key>
	<true/>
	<key>IDECodeSnippetVersion</key>
	<integer>2</integer>
</dict>
</plist>

