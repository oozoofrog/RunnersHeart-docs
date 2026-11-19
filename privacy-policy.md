# Privacy Policy

Updated November 18, 2026.

RunnersHeart records runs on Apple Watch and lets you review goals and workouts on iPhone. Core features do not require an account. The app operates no health-data server and sends no health or location data to advertising or analytics SDKs. Apple Maps, system sharing, and feedback email are described below.

## Health records

Apple HealthKit is the source of truth for workout data. RunnersHeart maintains no separate workout database, workout files, persistent summary replicas, or durable workout-message outbox. Displays and comparisons are derived from OS records. Your Apple Health and iCloud settings govern storage and synchronization of HealthKit originals.

Watch requests permission to read and write HealthKit workouts, heart rate, walking and running distance, active energy, and workout routes. During a workout, Watch uses the available heart rate, distance and energy measurements and session state. When you save, Watch stores the workout in HealthKit, with intervals and supported metadata for your goals, intensity choices and changes. For outdoor workouts, Watch uses authorized location observations to record a route in HealthKit when route writing is available. During a connected outdoor workout, Watch sends points added to the route to the paired iPhone. The in-app live map copies are kept in memory and cleared when the workout ends. Indoor runs do not collect a route.

iPhone requests HealthKit read access for workouts, heart rate, walking and running distance, active energy, workout routes, and workout effort. It uses the available workout dates, duration, distance, energy, average heart rate, intervals, goals, changes, recording source, routes, and effort ratings to display your records. iPhone requests write access for workouts and workout effort so it can request deletion of a workout you select and confirm, and save an effort sample you choose to link to a workout. Unanswered effort remains blank.

The app does not request date of birth, height, weight, resting heart rate, oxygen saturation, VO₂ max, or clinical records. It provides no numeric heart-rate target, diagnosis, or exercise clearance. Missing, stale, or failed observations are not replaced with invented measurements. An empty read result alone does not establish that you denied access.

## Device communication and system surfaces

The devices use HealthKit workout mirroring and WatchConnectivity to exchange current workout state, available measurements and their times, and change requests. Live route points travel through the mirrored HealthKit workout session. Prepared goals and cadence, sound and vibration settings also pass between devices. Watch controls the workout and confirms changes. The app does not keep a persistent queue of workout messages or relay them through its own server.

The iPhone app uses Apple Maps to load map imagery for the current route, saved routes, and the optional map on a workout card. The route is drawn over the map. Loading that imagery can use an internet connection.

Live Activities show confirmed current state. The iPhone widget queries OS workouts; the Watch goal widget reads your saved next-goal choice. System updates can be delayed. Stale heart rate is not displayed as a current measurement. Health values on system surfaces are marked sensitive; visibility also depends on system lock-screen and widget settings.

## App preferences

The app stores future goals, challenge, indoor or outdoor choice, cadence, and sound, voice and vibration settings in device preferences. Apps and widgets use the existing App Group to read needed goal choices. These preferences are not copies of active or completed workouts. Resetting settings resets choices on that device and preserves HealthKit workouts.

## Sharing, export, and deletion

When you share a workout, the app creates a card from the selected HealthKit record. An available outdoor route map is included by default and can be turned off before sharing. The map can show where a run began and ended. For sharing or saving an image to Photos, use the options available in the system share sheet. When you export CSV, the app uses the selected workout or displayed period. You choose recipients and storage locations through system controls. CSV output may include workout identifiers, dates, actual measurements, recording source, goals, intervals, changes, and saved effort. Current CSV exports exclude route coordinates and raw heart-rate sample arrays. Copies you save or send elsewhere must be managed at those destinations.

Deleting a workout requires separate confirmation in its details. The app requests deletion of that HealthKit workout within the permissions enforced by the OS. A failed deletion is not shown as success. Other records and the current active workout are outside that action. You can also manage original records and permissions in Health.

## Feedback email

The feedback button opens an editable email to the developer. The app fills in its version, your iPhone’s operating system and version, and the device type. You decide what to write, which details to keep, and whether to send the message using your mail app.

Troubleshooting logging is off by default. If you agree to turn it on in iPhone Settings, iPhone and its paired Watch keep recent app behavior events in their own caches for up to 7 days and up to 2,000 events per device. The log can include app and device information, settings, permission and connection status, event names and times, shortened workout IDs, and route recording counts. It excludes names, email addresses, text you type, raw heart-rate samples, and route points or coordinates.

You choose separately for each feedback email whether to attach the log. For that attachment, iPhone requests a report from the Watch if it is reachable and encrypts the file to the developer’s public key. If your mail app needs a manual attachment, you can share the encrypted file from Settings. The app does not automatically send the log to the developer.

Turning the setting off deletes the iPhone log and any pending attachment the app prepared for manual sharing. Watch deletes its log when it receives the change, including at the next contact if it was unreachable. The developer deletes received diagnostic files 90 days after handling the inquiry. For an earlier deletion request, email the contact address below. Copying the recipient address puts it on the iPhone clipboard.

## Permissions and choices

System controls let you grant or deny health and location access. Denial, unsupported features, or errors can restrict features or leave values unavailable. Without location access, a workout can still be recorded without a route. If only approximate location is allowed, Watch asks once at the start of an outdoor workout for precise location for that workout only; if you decline, the workout is recorded without a route. When you measure your cadence on Watch, the app reads your step count with Motion & Fitness access to suggest a cadence. With this access, it also uses step counts during a workout to detect when you stop moving. The app does not keep those step counts and saves the cadence you apply as a preference. Watch uses Apple’s speech synthesis to speak workout cues. It does not record microphone audio or use speech recognition.

Record comparisons show sample counts and comparison conditions. A single heart-rate change does not establish fitness improvement or safety. If urgent symptoms occur, stop exercising and prioritize appropriate help.

Development UI fixtures appear only when explicitly selected in a Debug Simulator build. They are not product records or evidence of HealthKit storage and are unavailable in Release.

Contact: [oozoofrog@oozoofrog.dev](mailto:oozoofrog@oozoofrog.dev)
