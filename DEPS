include_rules = [
  "+base",
  "+content/public/browser",
  "+content/public/common",
  "+content/public/test",
  "+components/keyed_service",
  "+components/user_prefs/pref_registry_syncable.h",
  "+components/web_modal",
  "+extensions",
  "+net/base",
  "+skia/ext",
  "+third_party/skia/include",
  "+ui",
  "+win8",

  # Temporary allowed includes.
  # TODO(benwells): remove these (http://crbug.com/159366)
  "+chrome/browser/chrome_notification_types.h",
  "+chrome/browser/chromeos/drive",
  "+chrome/browser/chromeos/login/user_manager.h",
  "+chrome/browser/lifetime/application_lifetime.h",
  "+chrome/browser/profiles",
  "+chrome/browser/sessions/session_id.h",
  "+chrome/common/chrome_switches.h",

  # Pieces of the extensions system that need to move to src/extensions.
  # See http://crbug.com/162530 for details.
  "+chrome/browser/extensions/api/app_runtime/app_runtime_api.h",
  "+chrome/browser/extensions/api/file_handlers/app_file_handler_util.h",
  "+chrome/browser/extensions/api/file_system/file_system_api.h",
  "+chrome/browser/extensions/extension_function_dispatcher.h",
  "+chrome/browser/extensions/extension_icon_image.h",
  "+chrome/browser/extensions/extension_host.h",
  "+chrome/browser/extensions/extension_web_contents_observer.h",
  "+chrome/browser/extensions/suggest_permission_util.h",
  "+chrome/browser/extensions/unpacked_installer.h",
  "+chrome/common/extensions/api/app_runtime.h",
  "+chrome/common/extensions/api/app_window.h",
  "+chrome/common/extensions/manifest_handlers/icons_handler.h",
]

specific_include_rules = {
  # Needs to be able to reload extensions. http://crbug.com/162530
  "app_load_service\.cc": [
    "+chrome/browser/extensions/extension_service.h",
  ],
  "(.*test\.cc|.*test_mac\.mm)": [
    "+chrome/browser/browser_shutdown.h",
    "+chrome/browser/extensions/extension_browsertest.h",
    "+chrome/browser/extensions/extension_test_message_listener.h",
    "+chrome/browser/extensions/test_extension_environment.h",
    "+chrome/browser/extensions/test_extension_prefs.h",
    "+chrome/browser/ui/browser.h",
    "+chrome/test/base/in_process_browser_test.h",
    "+chrome/test/base/interactive_test_utils.h",
    "+chrome/test/base/testing_profile.h",
    # Temporary allowed testing include.
    # TODO(benwells): Move app_browsertest_util into apps component once there
    # is an apps shell to test with.
    "+chrome/browser/apps/app_browsertest_util.h",
  ]
}
