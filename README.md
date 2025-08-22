# Antimatter Wiki

A collaborative wiki based on the [Antimatter Algorithm](https://braid.org/antimatter).

## Installation

```bash
npm install -g antimatter_wiki
```

## Quick Start

1. Run the wiki server:
```bash
antimatter_wiki
```

2. Open your browser and navigate to:
```
http://localhost:1001/any-page-name
```

3. Click the "edit" button in the lower-right, and edit the markdown in the textarea!

## Configuration

### Command Line Options

```bash
antimatter_wiki [port] [cert_file] [key_file]
```

| Parameter | Description | Default |
|-----------|-------------|---------|
| `port` | Port number to serve on | `1001` |
| `cert_file` | SSL certificate file for HTTPS | none |
| `key_file` | SSL key file for HTTPS | none |

### Examples

**Run on a different port:**
```bash
antimatter_wiki 8080
```

**Run with HTTPS:**
```bash
antimatter_wiki 443 /path/to/cert.pem /path/to/key.pem
```

## Data Storage

The wiki automatically creates and uses a `antimatter_wiki_db` directory in your current working directory to store all wiki pages and data.
