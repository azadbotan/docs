<!--
This file is auto-generated and will be re-generated every time the docs are updated.
To modify it, go to its source at https://github.com/fastlane/fastlane.
-->

# capture_ios_screenshots


Generate new localized screenshots on multiple devices (via _snapshot_)







capture_ios_screenshots |
-----|----
Supported platforms | ios, mac
Author | @KrauseFx



## 3 Examples

```ruby
capture_ios_screenshots
```

```ruby
snapshot # alias for "capture_ios_screenshots"
```

```ruby
capture_ios_screenshots(
  skip_open_summary: true,
  clean: true
)
```





## Parameters

Key | Description
----|------------
  `workspace` | Path the workspace file
  `project` | Path the project file
  `xcargs` | Pass additional arguments to xcodebuild for the test phase. Be sure to quote the setting names and values e.g. OTHER_LDFLAGS="-ObjC -lstdc++"
  `devices` | A list of devices you want to take the screenshots from
  `languages` | A list of languages which should be used
  `launch_arguments` | A list of launch arguments which should be used
  `output_directory` | The directory where to store the screenshots
  `output_simulator_logs` | If the logs generated by the app (e.g. using NSLog, perror, etc.) in the Simulator should be written to the output_directory
  `ios_version` | By default, the latest version should be used automatically. If you want to change it, do it here
  `skip_open_summary` | Don't open the HTML summary after running _snapshot_
  `skip_helper_version_check` | Do not check for most recent SnapshotHelper code
  `clear_previous_screenshots` | Enabling this option will automatically clear previously generated screenshots before running snapshot
  `reinstall_app` | Enabling this option will automatically uninstall the application before running it
  `erase_simulator` | Enabling this option will automatically erase the simulator before running the application
  `localize_simulator` | Enabling this option will configure the Simulator's system language
  `app_identifier` | The bundle identifier of the app to uninstall (only needed when enabling reinstall_app)
  `add_photos` | A list of photos that should be added to the simulator before running the application
  `add_videos` | A list of videos that should be added to the simulator before running the application
  `buildlog_path` | The directory where to store the build log
  `clean` | Should the project be cleaned before building it?
  `configuration` | The configuration to use when building the app. Defaults to 'Release'
  `xcpretty_args` | Additional xcpretty arguments
  `sdk` | The SDK that should be used for building the application
  `scheme` | The scheme you want to use, this must be the scheme for the UI Tests
  `number_of_retries` | The number of times a test can fail before snapshot should stop retrying
  `stop_after_first_error` | Should snapshot stop immediately after the tests completely failed on one device?
  `derived_data_path` | The directory where build products and other derived data will go
  `test_target_name` | The name of the target you want to test (if you desire to override the Target Application from Xcode)
  `namespace_log_files` | Separate the log files per device and per language
  `concurrent_simulators` | Take snapshots on multiple simulators concurrently. Note: This option is only applicable when running against Xcode 9




<hr />
To show the documentation in your terminal, run
```no-highlight
fastlane action capture_ios_screenshots
```

<a href="https://github.com/fastlane/fastlane/blob/master/fastlane/lib/fastlane/actions/capture_ios_screenshots.rb" target="_blank">View source code</a>

<hr />

<a href="/actions"><b>Back to actions</b></a>
