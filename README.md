# Checkpoint Google Tag Manager Template

This repository contains the official Google Tag Manager (GTM) template for Checkpoint, the AI agent identity & protection platform from [KnowThat.ai](https://kya.vouched.id). It detects and identifies AI agents and automated bot traffic accessing your website.

## Quick Installation

### Method 1: Import from Repository (Recommended)

1. Download the `template.tpl` file from this repository
2. In Google Tag Manager, go to **Templates** → **Tag Templates**
3. Click **New** → **Import**
4. Select the downloaded `template.tpl` file
5. Save the template

### Method 2: Community Template Gallery (Coming Soon)

1. In GTM, go to **Templates** → **Tag Templates**
2. Click **Search Gallery**
3. Search for "Checkpoint"
4. Click **Add to Workspace**

## Creating a Tag

After importing the template:

1. Go to **Tags** → **New**
2. Click **Tag Configuration**
3. Select **Checkpoint Pixel** from Custom templates
4. Configure the required settings:
   - **Project ID**: Your Checkpoint project ID (required)
   - **API Endpoint**: Custom endpoint URL (optional)
   - **Debug Mode**: Enable for testing (optional)
   - **Session Timeout**: Session duration in milliseconds (default: 1800000)
   - **Respect Do Not Track**: Honor user DNT preference (default: true)
   - **Batch Size**: Events per batch (default: 10)
   - **Flush Interval**: Batch flush frequency in ms (default: 5000)
   - **Enable Fingerprinting**: Advanced detection (default: true)

## Configuration Parameters

| Parameter | Type | Required | Default | Description |
|-----------|------|----------|---------|-------------|
| Project ID | Text | Yes | - | Your Checkpoint project identifier |
| API Endpoint | Text | No | Auto-detected | Custom API endpoint URL |
| Debug Mode | Checkbox | No | false | Enable console debugging |
| Session Timeout | Number | No | 1800000 | Session timeout in milliseconds |
| Respect Do Not Track | Checkbox | No | true | Honor browser DNT setting |
| Batch Size | Number | No | 10 | Number of events per batch |
| Flush Interval | Number | No | 5000 | Batch flush interval in ms |
| Enable Fingerprinting | Checkbox | No | true | Advanced browser detection |

## Setting Up Triggers

Configure triggers based on your needs:

- **All Pages**: Basic protection across your site
- **Form Submissions**: Protect contact forms and signups
- **Button Clicks**: Track specific user interactions
- **Custom Events**: Advanced tracking scenarios

## Testing Your Installation

1. Use GTM's **Preview** mode
2. Check the browser console for Checkpoint debug messages
3. Verify events are being sent to Checkpoint
4. Monitor the Checkpoint dashboard for activity

## Troubleshooting

### Template Not Loading
- Ensure the template was imported correctly
- Check that all required parameters are configured
- Verify your GTM container is published

### No Data in Checkpoint Dashboard
- Confirm your Project ID is correct
- Check that triggers are firing
- Enable debug mode to see console logs
- Verify your website has traffic

### JavaScript Errors
- Check browser console for error messages
- Ensure no ad blockers are interfering
- Verify Content Security Policy allows Checkpoint domains

## Support

For questions or issues:

- **Documentation**: [https://kya.vouched.id/docs](https://kya.vouched.id/docs)
- **GitHub Issues**: [Report template issues here](https://github.com/Know-That-Ai/checkpoint-gtm-template/issues)

## License

This template is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for improvements.

---

**Note**: This template requires an active Checkpoint account. Get started at [https://kya.vouched.id](https://kya.vouched.id).