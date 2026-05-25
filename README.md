#  Eye & Water Reminder App


_A simple yet powerful reminder app to take care of your **eye health** and **hydration needs**._

---

## 📱 About the App
Eye & Water Reminder is an Android application designed to remind users to:
- Take regular **eye breaks** (reducing digital strain).
- Drink enough **water** throughout the day.

---

## 🚀 Features
✅ Smart reminders for both **eye breaks** & **water intake**  
✅ Customizable reminder frequency  
✅ User-friendly **UI with Material Design**  
✅ Lightweight & battery-efficient  

---

## 🛠 Tech Stack
- **Language**: Kotlin
- **Architecture**: MVVM (Model-View-ViewModel) with Clean Architecture 
- **UI Toolkit**: Jetpack Compose
- **Local Storage**: Room Database
- **Dependency Injection**: Hilt
- **Async & Reactive**: Coroutines & Flow
- **Background Tasks**: WorkManager

---

```

com.alpha.myeyecare/ 
│ 
├── common/                          
│   ├── constants/ 
│   │   ├── AppDestinations.kt
│   │   └── ReminderTypes.kt 
│   └── utils/ 
│       ├── ExtensionFunctions.kt            
│       └── UtilFunctions.kt         
│ 
├── data/                            
│   ├── local/                       
│   │   ├── converters/ 
│   │   │   ├── Converters.kt 
│   │   ├── dao/ 
│   │   │   ├── ReminderDao.kt  
│   │   ├── entities/ 
│   │   │   ├── Reminder.kt  
│   │   └── ReminderDatabase.kt 
│   │ 
│   └── repository/                 # Repository implementation
│       ├── SuggectionRepositoryImpl.kt  
│       └── ReminderRepositoryImpl.kt  
│  
├── di/                             
│   ├── AppModule.kt 
│   ├── DatabaseModule.kt
│   └── RemoteModule.kt 
│
├── domain/                         
│   ├── model/ 
│   │   ├── DaysOfWeek.kt 
│   │   ├── ReminderDetails.kt 
│   │   ├── ReminderFrequency.kt 
│   │   └── Suggestion.kt 
│   │ 
│   ├── repository/                 # Abstract repository interfaces 
│   │   ├── ReminderRepository.kt 
│   │   └── SuggestionRepository.kt 
│   │ 
│   └── usecase/                   
│       ├── CheckReminderStatusUseCase.kt 
│       ├── GetReminderDetailsUserCase.kt 
│       ├── SaveReminderUseCase.kt  
│       └── SaveSuggestionsUseCase.kt 
│ 
├── presentation/                  
│   ├── navigation/ 
│   │    └── NavGraph.kt  
│   └── ui/                   
│       ├── common/ 
│       │   └── CommonUI.kt
│       ├── detailsScreen/ 
│       │   ├── SetupReminderScreen.kt
│       │   └── SetupReminderViewModel.kt
│       ├── home/ 
│       │   └── HomeScreen.kt 
│       ├── splash/ 
│       │   ├── SplashScreen.kt
│       │   └── SplashViewModel.kt 
│       ├── suggestion/ 
│       │   ├── SuggestionSubmissionViewModel.kt 
│       │   └── UserSuggestionScreen.kt
│       ├── theme/ 
│       │   ├── Color.kt 
│       │   ├── Theme.kt 
│       │   └── Type.kt 
│       └── userPermission.kt  
├── Worker/                  
│   ├── ReminderScheduler.kt
│   └── ReminderWorker.kt 
├── MainActivity.kt                   
└── MyApplication.kt                 

```

