flowchart TD
    A[شروع] --> B[فاز شناسایی]
    B --> B1[Subfinder: زیردامنه‌ها]
    B --> B2[Nmap: پورت‌های باز]
    B --> B3[Httpx: بررسی زنده بودن]
    
    B1 & B2 & B3 --> C[فاز اسکن]
    C --> C1[Nuclei: 1000+ تست خودکار]
    C --> C2[SQLi پیشرفته: Time-based]
    C --> C3[XSS پیشرفته: Pattern match]
    C --> C4[SSRF & SSTI]
    
    C1 & C2 & C3 & C4 --> D[فاز تحلیل]
    D --> E[گزارش با راه‌حل رفع]
