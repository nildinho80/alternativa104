{
  "manifest_version": 3,
  "name": "Assistente de Texto",
  "version": "1.0.0",
  "description": "Extensão de exemplo para melhorar textos.",
  "permissions": [
    "storage",
    "activeTab",
    "scripting"
  ],
  "host_permissions": [
    "https:///"
  ],
  "background": {
    "service_worker": "background.js"
  },
  "action": {
    "default_popup": "popup.html",
    "default_title": "Assistente de Texto"
  },
  "options_page": "options.html",
  "content_scripts": [
    {
      "matches": ["https:///"],
      "js": ["content.js"]
    }
  ]
}
