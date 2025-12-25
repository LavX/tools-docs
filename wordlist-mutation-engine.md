# Wordlist Mutation Engine

Generate powerful password mutations for security research and authorized penetration testing.

The **Wordlist Mutation Engine** is a comprehensive security research tool designed for password security analysis and authorized penetration testing. It provides a sophisticated rule-based system to generate password variations from base words, supporting industry-standard formats like Hashcat and John the Ripper.

## Key Features

### 🎯 Visual Rule Builder
- **Interactive Interface**: Build mutation chains visually with drag-and-drop functionality
- **Real-time Preview**: See mutation results instantly as you modify rules
- **Rule Management**: Add, remove, reorder, and toggle individual rules
- **Auto-generation**: Automatically generates mutations as rules change

### 📚 Template Library
- **Pre-built Templates**: Ready-to-use rule combinations for common scenarios
- **Categories**: Password cracking, corporate, personal, social media, leet variations, keyboard patterns, year/date patterns
- **One-click Application**: Apply entire template sets instantly

### 📊 Batch Processing
- **Multiple Export Formats**: Plain text, Hashcat rules, John the Ripper rules, JSON
- **Customizable Limits**: Configure maximum outputs, deduplication, sorting
- **Progress Tracking**: Monitor batch processing with progress indicators

### 🔒 Security Features
- **Rate Limiting**: Built-in protection against abuse (30 mutations/minute for single words, 10/minute for batch processing)
- **Input Validation**: Safe handling of user inputs and regex patterns
- **Privacy First**: All processing happens client-side in your browser

### 🎨 Rich Rule System
- **80+ Rules**: Comprehensive set of mutation rules across 9 categories
- **Categories Include**:
  - **Leet Speak** (11 rules): Letter-to-number/symbol substitutions (a→4, e→3, i→1, o→0, s→5, etc.)
  - **Case Mutations** (9 rules): Lowercase, uppercase, capitalize, toggle, alternate, invert first
  - **Suffixes** (21 rules): Append numbers, years, special characters
  - **Prefixes** (12 rules): Prepend common words, numbers, symbols
  - **Substitutions** (12 rules): Find-and-replace with regex support
  - **Transforms** (10 rules): Reverse, duplicate, rotate, reflect operations
  - **Deletions** (13 rules): Remove characters, truncate operations
  - **Insertions** (12 rules): Add characters at specific positions
  - **Special Patterns** (11 rules): Year ranges, sequential patterns, keyboard walks

## Rule Categories

### Leet Speak (11 rules)
- Basic substitutions: a→4, e→3, i→1, o→0, s→5
- Extended leet with additional character mappings
- Symbol-heavy variants: a→@, s→$, i→!
- Single-character transformations

### Case Mutations (9 rules)
- Convert to lowercase/uppercase
- Capitalize first letter
- Toggle each character's case
- Alternate case patterns
- Invert first letter case

### Suffixes (21 rules)
- Append numbers (1, 123, 2015-2025)
- Special characters (!, @, #, $, etc.)
- Common patterns and sequences

### Prefixes (12 rules)
- Append common suffixes (!, #, 123, 2023)
- Prepend prefixes (Mr, Ms, Dr)
- Year ranges (1990-2023)
- Custom character patterns

### Substitution Rules (12 rules)
- Character replacement (custom find/replace)
- Global substitutions
- Regex-based substitutions

### Transform Rules (10 rules)
- Reverse word order
- Duplicate operations (word, first/last character)
- Left/right rotation
- Reflect (word+reverse)

### Deletions (13 rules)
- Remove characters from positions
- Delete first/last characters
- Truncate operations
- Keep-first-N operations

### Insertions (12 rules)
- Insert characters at start/end/specific position
- Delete first/last characters
- Truncate operations
- Position-based modifications

### Special Patterns (11 rules)
- Year suffix ranges (1990-2025)
- Keyboard walk patterns
- Sequential numbers and patterns
- Lucky numbers and sequences

## Usage

### Basic Word Mutations
1. Navigate to the [Wordlist Mutation Engine](https://tools.lavx.hu/tools/wordlist-mutation-engine)
2. Enter a base word (e.g., "password")
3. Add rules from the Rule Palette by clicking on them
4. View real-time preview of generated mutations
5. Click "Generate" to create full mutation set
6. Export results in your preferred format

### Batch Processing
1. Switch to the "Batch Processor" tab
2. Upload or paste your wordlist (one word per line)
3. Configure rules using the Rule Builder
4. Process the entire wordlist
5. Export results as plain text, Hashcat rules, or John the Ripper rules

### Template Library Usage
1. Go to the "Template Library" tab
2. Browse templates by category:
   - **Password Cracking**: Common password patterns
   - **Corporate**: Company name variations
   - **Personal**: Name + DOB combinations
   - **Social Media**: Username patterns
   - **Leet Variations**: Number substitutions
   - **Keyboard Patterns**: Sequential patterns
   - **Year/Date**: Date appendages
3. Apply templates with one click
4. Customize rules as needed

## How It Works

The Wordlist Mutation Engine uses a sophisticated **combinatorial approach** to generate mutations. Unlike simple sequential rule application, it creates **all possible combinations** of your enabled rules using a power-set algorithm:

### Combinatorial Mutations
- **Power Set Generation**: For N enabled rules, generates up to 2^N - 1 rule combinations
- **Combination Application**: Each subset of rules is applied sequentially to the input word
- **Limit Protection**: Configurable maximum output limits prevent exponential explosion
- **Result Optimization**: Deduplication and sorting applied to final results

### Example (Combinatorial vs Sequential)
**Input**: `password`
**Rules**: `Lowercase`, `Reverse`, `Add '1'`

**Sequential** (one rule at a time):
- Lowercase → `password` (no change)
- Reverse → `ssrowssap`
- Add '1' → `password1`

**Combinatorial** (all combinations):
- Lowercase → `password`
- Reverse → `sswordpass`
- Add '1' → `password1`
- Lowercase+Reverse → `ssrowssap`
- Reverse+Lowercase → `ssrowssap` (same)
- Add '1'+Lowercase → `password1` (same)
- Lowercase+Reverse+Add '1' → `ssrowssap1`
- **Total**: 7 unique mutations

## Technical Specifications

### Input Limits
- **Single Word**: Maximum 100 characters
- **Wordlist**: Maximum 10,000 words
- **Rules**: Maximum 20 rules per mutation chain
- **Preview**: Maximum 20 mutations shown

### Output Controls
- **Max Outputs**: Configurable (default: 10,000)
- **Deduplication**: Automatic removal of duplicates
- **Sorting**: Optional alphabetical sorting
- **Original Preservation**: Option to include original words

### Export Formats
1. **Plain Text**: Simple wordlist format
2. **Hashcat Rules**: Industry-standard `.rule` files
3. **John the Ripper**: `.john` rule files
4. **JSON**: Structured data with metadata and statistics

### Unimplemented Rules
Some rule types are defined but not fully implemented:
- **KEYBOARD_WALK**: Complex keyboard pattern generation (use suffix/prefix rules instead)
- **OVERSTRIKE**: Legacy terminal effect (limited practical use)

### Performance
- Real-time preview generation (300ms debouncing)
- Efficient parallel rule application
- Optimized for large wordlists
- Browser-side processing (no server dependencies)
- Rate limiting: 30 mutations/minute (single words), 10/minute (batch)

## Security Disclaimer

**This tool is designed for authorized security testing and penetration testing only.** 

- **Authorized Use Only**: Use only on systems you own or have explicit permission to test
- **Legal Compliance**: Users are responsible for ensuring their usage complies with applicable laws and regulations
- **Educational Purpose**: Intended for security awareness and authorized penetration testing
- **Misuse Warning**: Unauthorized use may violate laws and regulations

## Examples

### Example 1: Basic Password Variations
**Input**: `password`
**Rules**: Basic Leet + Case Toggle
**Output**: `p4ssw0rd`, `P4SSW0RD`

### Example 2: Corporate Wordlist
**Input**: `company`
**Rules**: Case Variations + Year Suffixes (2020-2023)
**Output**: `Company2020`, `company2021`, `COMPANY2022`, `Company2023`

### Example 3: Personal Information Mutations
**Input**: `john`
**Rules**: Basic Leet + Common Suffixes
**Output**: `j0hn123`, `john!`, `j0hn2023`

## Integration

The Wordlist Mutation Engine supports integration with:
- **Hashcat**: Export compatible `.rule` files
- **John the Ripper**: Export `.john` rule files  
- **Password Crackers**: Plain text wordlist exports
- **Security Tools**: JSON format for custom integrations

---

**Access the tool**: [https://tools.lavx.hu/tools/wordlist-mutation-engine](https://tools.lavx.hu/tools/wordlist-mutation-engine)

**Explore more tools**: [tools.lavx.hu](https://tools.lavx.hu)