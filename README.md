# SCV
Sublime Cool Version are configurations for Sublime Text 3 and PHP developers, inspired in Laravel community.

## Installation
1. Clone this repo into Sublime Text Packages directory. Preferences -> Browse Packages...
2. Copy all files from SCV/User to Packages/User.
3. Install the next packages.

### Packages
Install with Package Control

+ SideBarEnhancements
+ DocBlockr
+ AdvancedNewFile
+ Dayle Rees Color Schemes
+ Markdown Preview

Optional
+ PackageResourceViewer
+ PHP Getters and Setters

## Final Files Structure
    Packages
    ├── SCV
    │   ├── Snippets
    │   │   ├── class_extends.sublime-snippet
    │   │   ├── class_implements.sublime-snippet
    │   │   ├── class-laravel-testcase.sublime-snippet
    │   │   ├── class-phpunit.sublime-snippet
    │   │   ├── class.sublime-snippet
    │   │   ├── interface_private_function.sublime-snippet
    │   │   ├── interface_protected_function .sublime-snippet
    │   │   ├── interface_public_function.sublime-snippet
    │   │   ├── interface.sublime-snippet
    │   │   ├── private_function.sublime-snippet
    │   │   ├── protected_function.sublime-snippet
    │   │   ├── public_function.sublime-snippet
    │   │   └── trait.sublime-snippet
    │   ├── User
    │   │   ├── Base File.sublime-settings
    │   │   └── Preferences.sublime-settings
    │   ├── Default (Linux).sublime-keymap
    │   ├── Default (Linux).sublime-mousemap
    │   └── README.md
    └── User
        ├── Base File.sublime-settings
        └── Preferences.sublime-settings


## Sublime Text User preferences
File

    Preferences.sublime-settings

Options
+ Theme like Laravel's website.
+ Line spacing like Taylor Otwell.
+ 80 characters rule
+ Translate tabs to spaces


## DocBlockr User Preferences
File

    Base File.sublime-settings

Generate documentation like this:

    /**
     * [sendSmsMessage description]
     *
     * @param  SmsCourierInterface $courier
     * @param  [type] $message
     * @return [type]
     */
    public function sendSmsMessage(SmsCourierInterface $courier, $message)
    {
        $courier->sendMessage($this->phone_number, $message);

        return $this->sms()->create([
            'to' => $this->phone_number,
            'message' => $message;
        ]);     
    }

## Snippets

| Key binding | Description |
|----------|------|
| cc + tab | class |
| ci + tab | class implements |
| ce + tab | class extends |
| ct + tab | class extends TestCase (Laravel) |
| cp + tab | class extends PHPUnit_Framework_TestCase |
| ii + tab | interface |
| tt + tab | trait |
| pubf + tab | public function |
| prof + tab | protected function |
| prif + tab | private function |
| ipubf + tab | inline public function definition |
| iprof + tab | inline protected function definition |
| iprif + tab | inline private function definition |
