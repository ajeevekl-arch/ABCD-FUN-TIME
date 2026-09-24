#!/system/bin/sh
if command -v gradle >/dev/null 2>&1; then
  exec gradle "$@"
fi
if [ -x "$HOME/.gradle/bin/gradle" ]; then
  exec "$HOME/.gradle/bin/gradle" "$@"
fi
echo "Gradle is not installed. In AndroidIDE Terminal run: idesetup -c"
exit 127
