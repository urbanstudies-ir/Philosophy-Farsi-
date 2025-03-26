# 📦 DDP Knowledge Graph Action | اکشن گراف دانش DDP

A GitHub Action for processing philosophical concepts into RDF/OWL knowledge graphs with support for Farsi and English, SKOS classification, and DDP API integration.

اکشنی برای تولید گراف مفهومی RDF/OWL از مفاهیم فلسفی، با پشتیبانی فارسی/انگلیسی، طبقه‌بندی SKOS و اتصال به API رسمی DDP.

## 🚀 Features | ویژگی‌ها

- Dual-language support (FA/EN) | پشتیبانی دوزبانه
- Converts conceptual entries to RDF/OWL | تبدیل مفاهیم به RDF/OWL
- Compatible with Protégé, GraphDB, Neo4j | سازگار با ابزارهای فلسفی
- Standard metadata (SKOS, Dublin Core) | متادیتای استاندارد
- Linked to DDP OpenAPI 3.0 | اتصال به API DDP

## 🧠 Use Case Example | نمونه استفاده

```yaml
name: Generate DDP RDF Graph
on:
  push:
    paths:
      - 'concepts/*.json'

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout code
        uses: actions/checkout@v3

      - name: Run RDF Conversion
        uses: urbanstudies-ir/Philosophy-Farsi-@v1
        with:
          input_path: concepts/
          output_format: turtle
```

## 🔐 Privacy Policy

No user data is collected.  
📄 [Privacy Policy](https://urbanstudies-ir.github.io/Philosophy-Farsi-/privacy-policy.html)

## 📝 License

MIT © urbanstudies-ir
