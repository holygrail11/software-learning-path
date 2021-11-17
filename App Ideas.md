# App Ideas

**1. Beginner**

* Blog (Web)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E.
        * Database - SQL/NoSQL  

* Weather app / Dark skies clone (Web)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * Database - SQL/NoSQL
        * Client-Server architecture - Separate API(Backend) and App(Frontend)
        * External API Integration : Accuweather etc 
        * Location services integrations : Google maps        

**2. Intermediate**

* Chat App (Web)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * Database - NoSQL 
        * Client-Server architecture - Separate API(Backend) and App(Frontend)
        * Websockets 
        * Pusher
        
* Log Files Reader (Web)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * Database - NoSQL
        * Client-Server architecture - Separate API(Backend) and App(Frontend)  
        * Websockets
        * Filesystem
        * Streaming
        * Async-processing: Consumers/Daemons
        
* Log Notifications Library (Web)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * External API Integration: Email, SMS, Web Push Notifications, Slack   
        * Async Processing: Queues
        * Software Library development   
        
* Web scrapper (Web)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * Database - NoSQL
        * External API Integration: Email, Web Push Notifications   
        * Web scrapping 
        * Client-Server architecture - Separate API(Backend) and App(Frontend)
    * Features/Requirements:
        * Scrap websites eg news websites
        * Send notifications from scrapped information       

* Classwork Management System / Google class/Skoolspace clone (Web)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * Database - SQL/NoSQL 
        * Client-Server architecture - Separate API(Backend) and App(Frontend)
        * External API Integration: Email, Web Push Notifications, Google Calendar   
        * Search - Elasticsearch/Fulltext search 
        * File system - Storage, Deduplication(Efficient storage)
        * 3rd Party Authentication
        * OCR
        * Async-processing: Queues/DB Events
    * Features/Requirements:
        * Users can signup via email and a password 
        * Users can sign in via Google account (possible linked to their school email)
        * Have an admin who can be the class rep
        * Admin can add people to his class/accept requests to join
        * Users can request to join a class
        * A class can have a shared folder/space containing:
          announcements, reminders, files (notes etc),
          assignments, calendar.
        * Assignments can have title and due date. A reminder
          can be set when creating an assignment.  
        * Users have 'backpack' which contains personal:
          reminders, notes, files 
        * Reminders can be sent via email or web push
        * Calendar showing timetable, upcoming events (e.g assignments)
        * Users can search for other users, files, notes
        * Users can share their content e.g files
        * Notes can be: PDF, Doc, Powerpoint, Images, Zip
        * Notes: Image upload (take photos of notes and OCR the content, then index)
        * Scrap through uploaded notes files and index the data
        * Searchable Glossary of common terms e.g unit names(use Elastic search), 

**3. Advanced**

* Log Files Reader (CLI)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * CLI (Command Line Interface) Apps
        * Database - NoSQL  
        * Websockets
        * Filesystem
        * Streaming
        * Async-processing: Consumers/Daemons

* Online Code Editor / CodeSandbox clone (Web)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * Database - NoSQL  
        * File system - Storage, Syncing(files edited on different devices at different times, eg shared docs)      

* Video streamer / Youtube/Vimeo clone (Web)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * Database - SQL/NoSQL 
        * Client-Server architecture - Separate API(Backend) and App(Frontend)
        * Memory Intensive Applications  
        * Streaming - Buffering techniques
        * Search - Elasticsearch/Fulltext search
        * File system - Storage, Deduplication(Efficient storage)
        * Video codec
        * Video processing
        * Async processing - Queues
    * Features/Requirements:
        * Upload videos
        * CRUD operations
        * Store video in different codecs, formats, resolutions (Advanced requirement). 
         This can be done via async-processing.
        * Index video metadata eg title
        * Stream videos
        * Search for videos e.g by title
        * Captions/Transcription (Advanced requirement)           

* Image management app / Flickr/Google photos clone (Web)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * Database - SQL/NoSQL 
        * Client-Server architecture - Separate API(Backend) and App(Frontend)
        * Search - Elasticsearch/Fulltext search
        * File system - Storage, Deduplication(Efficient storage)
        * Photo codecs/formats
        * Compression algorithms
        * OCR
        * Async processing - Queues, Web-workers
        * External API Integration: Email, Offensive images API, Bitly   
    * Features/Requirements:
        * Upload photos, either single, or a bunch
        * CRUD operations
        * Generate links to images to share via email. Use Bitly or own solution.
        * Users can see list of their photos in a gallery like format
          with different filters e.g by date, size, title
        * Compress photos for efficient storage (e.g https://squoosh.app/editor). 
          Use web-workers (https://www.youtube.com/watch?v=7Rrv9qFMWNM)
        * User can add filters to photos
        * User can change format eg, from jpg to png
        * Store photos in different formats (Advanced requirement)
        * Index photo metadata eg title
        * Use OCR to get any text-in-image and index it
        * Search for photos e.g by title, by text in image
        * Block offensive images. Use queues to either look up an 
          uploaded image against an external offensive images API or an internal record.
        
* Peer-to-Peer file sharing app / uTorrent/mega clone (Web/Desktop)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * Database - SQL/NoSQL 
        * Client-Server architecture - Separate API(Backend) and App(Frontend)
        * Peer-to-peer networking/resource sharing
        * File system - Syncing(local and online/files edited on different devices at different times, eg shared videos/docs)      
    * Features/Requirements:
        * Users to have local and cloud folders with their content
        * Upload and share files
        * Download files from other peers active in the network
        * Pause and resume downloads
        * Check estimated download time 
        * Limit downloads per user eg (max of 2GB per user per day)
        * Manage peers and their resources in the network.
          For example if a peer drops off/deletes a file that was served to others,
          how do you handle that.   

* Peer-to-Peer file sharing app / uTorrent/mega clone (CLI)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * Database - SQL/NoSQL 
        * CLI (Command Line Interface) Apps 
        * Peer-to-peer networking/resource sharing
        * File system - Syncing(files edited on different devices at different times, eg shared docs)     
    * Features/Requirements: Same as for the Web/Desktop versions     

* Bulk/Mass Notification Gateway (Web)
    * Github Link:
    * Technologies/Concepts:
        * Software Testing - Unit, Integration, Functional, E2E
        * Database - SQL/NoSQL 
        * Client-Server architecture - Separate API(Backend) and App(Frontend)
        * Async processing - Queues
        * External API Integration: Email(eg Sendgrid, Mailgun), SMS (e.g Twillio)
        * Bulk transactions/Transaction-heavy systems
        * Payments integration (** advanced requirement)      
    * Features/Requirements: 
        * Sends emails/SMSes to multiple groups of people
        * User can upload a CSV containing contacts(emails, phone nos.)
        * System extracts and saves user's CSV as a contact list
        * User can send messages to contacts
        * CRUD operations
        * User is billed for usage/payments integration (**advanced requirement)

