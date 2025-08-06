# Security-concepts

### CIA Triad , Zero trust & **[Physical security ](https://github.com/sherazi1214/physical-security/new/main?readme=1):**
CIA stands for:

Confidentiality (رازداری)

Integrity (درستگی)

Availability (دستیابی)

These 3 pillars define how we protect data.

## Confidentiality (رازداری)
##### Meaning (English):
Confidentiality means ensuring that only authorized people can access sensitive information. It protects data from unauthorized access.

 ##### Meaning (Urdu):
Confidentiality ka matlab hai ke sirf authorized (ijazat shuda) log hi kisi maloomat tak pohonch sakain. Yeh data ko ghair mutaliqa logon se bachata hai.

#### Examples:

Passwords and biometrics

Data encryption

Access control lists (ACLs)

## Integrity (درستگی / اصلیت)
##### Meaning (English):
Integrity means ensuring that data is accurate and unaltered. No one should be able to change data without permission.

##### Meaning (Urdu):
Integrity ka matlab hai ke data bilkul theek, original aur unchanged ho. Koi bhi shakhs data ko bina ijazat tabdeel (modify) nahi kar sakta.

### Examples:

Hashing (to verify data)

Digital signatures

Checksums

### Availability (دستیابی)
##### Meaning (English):
Availability means that authorized users can access data or systems whenever they need it, without delay.

##### Meaning (Urdu):
Availability ka matlab hai ke jo log ijazat rakhte hain, woh system ya maloomat tak har waqt asani se pohonch sakain.

### Examples:

Redundant servers

Backup systems

UPS/power protection

## CIA Triad Summary Table
Concept ------------------------	Meaning (EN) ------------------------	Urdu Meaning ------------------------	-Main Goal

Confidentiality-----------------	Keep data secret -------------------	Data ko sirf authorized log dekhein ---	Prevent unauthorized access

Integrity ----------------------	Keep data accurate and unchanged ---	Data sahi aur tabdeel na ho ----------	Prevent tampering

Availability -------------------	Keep data/system always usable ------	Data hamesha available ho	 -------------Prevent downtime



## What is Privacy? 
##### Privacy (English):
Privacy means protecting a person’s personal information from being exposed, misused, or accessed without their consent.

##### Privacy (Urdu):
Privacy ka matlab hai kisi shakhs ke zati maloomat (personal data) ko is tarah mehfooz rakhna ke bina uski ijazat ke koi use access na kare ya misuse na kare.

### Privacy Examples:

Protecting your name, address, ID, phone number

Hiding your online activity from tracking

GDPR law in Europe (protects personal privacy)

 Privacy relates closely to confidentiality, but:

Confidentiality = data protection

Privacy = personal rights and consent


## What is Zero Trust?
#### English:
Zero Trust is a modern security model that means:

“Never trust, always verify.”

Even if a device or user is inside the network, they must still be continuously verified before accessing anything.

#### Urdu:
Zero Trust ek aisa security model hai jisme:

"Kisi par bhi andha bharosa nahi — hamesha verify karo."

Yeh assume karta hai ke har user, device, ya application potentially unsafe ho sakta hai — chahe woh network ke andar hi kyun na ho.

## Zero Trust  Principles
**Verify explicitly** (Always check who is asking)

Har request ko authenticate karo (multi-factor, biometrics)

**Least privilege access** (Give minimum required access)

User ko sirf wohi access milay jo zaroori ho

**Assume breach** (Expect attacks)

Har device ya user ko potentially compromised samjho

## Zero Trust Logical Components (Full Detail)
### Component ------------------------------------	Explanation (English + Urdu)

### Identity Provider -----------------------------	 Confirms who the user is (username/password, MFA).
📙 Yeh batata hai ke user asal mein kaun hai.	

### Device Security	------------------------------ Checks if the device is secure, patched, and trusted.
📙 Yeh ensure karta hai ke system ya phone secure hai.	

### Network Segmentation	------------------------- Breaks the network into smaller zones to control traffic.
📙 Network ko choti zones mein divide karta hai taake access limit ho.	

### Policy Engine	------------------------------- Decides whether to allow or deny access.
📙 Rules ke mutabiq decision leta hai ke access dena hai ya nahi.	

### Policy Enforcement Point (PEP)	-------------- Executes the decision made by the policy engine.
📙 Access ko allow ya block karne ka actual point hota hai.	

### Continuous Monitoring	------------------------ Monitors behavior, location, risk level, etc.
📙 Hamesha check karta hai ke kuch unusual to nahi ho raha.

### Analytics and Automation	--------------------- Uses AI/ML to detect threats and respond.
📙 Smart tools jo khud se threat detect aur response karti hain.


### **Control Plane**
The "brain" – where policies and decisions are made. It manages authentication, authorization, and rules.
#### simple
Control Plane woh jagah hai jahan decision liya jata hai ke access dena hai ya nahi.

### **Data Plane**
The "path" – where actual data flows and is transferred. It enforces what was decided by the control plane.

### simple 
Data Plane woh jagah hai jahan asli data ka safar hota hai, jaise file transfer ya web access.

 ### Real-World Example (Easy Scenario):
Imagine you're accessing your office app from your laptop.

**Identity Provider**: Confirms you’re really you (via 2FA)

**Device Check**: Ensures your laptop is secure and updated

**Policy Engine**: Applies company rules (e.g., working hours only)

**Control Plane**: Verifies your ID, device, location, time

**Policy Enforcement Point**: Allows/block your request

**Data Plane**: You download the document (actual data access)

**Continuous Monitoring**: System watches your behavior during access

## Summary Table:
### Concept ---------------------------------------------	Meaning

### Zero Trust ---------------------------------------------	Security model: "Never trust, always verify"

### Control Plane -----------------------------------------	Makes decisions (verify, allow, deny)

### Data Plane --------------------------------------------	Transfers actual data (files, access)

### Logical Components ------------------------------------	Tools and systems that make Zero Trust work (identity, policy engine, device checks, etc.)
