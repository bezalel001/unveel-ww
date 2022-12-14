# Unveel Weather Widget

A react weather component library ![unveel-ww-themes](https://user-images.githubusercontent.com/11287142/185853886-b8c849a1-3a61-42c9-9187-fbc4cf3eaf40.png)

# ☁️ unveel-ww ☁️

### Installation

### `see development`

### ✨ Features

-   Typescript Support
-   Customizable Theme (Dark and Light)
-   Refreshes Data in the background - Updates data periodically in the background

### ☁️ Peer Dependencies

-   "react": "^18.2.0"
-   "react-dom": "^18.2.0"
-   "styled-components": "^5.3.5"
-   "styled-theming": "^2.2.0"

### ☁️ Usage

-   Basic

    ```JSX
    import React from 'react';
    import { UWeatherWidget } from '@bezalel001/unveel-ww';

    const BasicComponent = () => {

      const apiKey= 'xxx'; // your openweathermap api key

      return (
        <UWeatherWidget openWeatherAPIKey={key} />
      );
    }
    ```

-   Refresh Data in the Background

    ```JSX
    import React from 'react';
    import { UWeatherWidget } from '@bezalel001/unveel-ww';

    const ReloadData = () => {

      const key = 'xxx'; // your openweathermap api key

      return (
        <UWeatherWidget
          openWeatherAPIKey={key}
          periodicallyRefreshDataInSeconds={60}
        />
      );
    }
    ```

-   Light Theme

    ```JSX
    import React from 'react';
    import { UWeatherWidget } from '@bezalel001/unveel-ww';

    const LightTheme =() => {

      const key = 'some key'; // your openweathermap api key

      return (
        <UWeatherWidget
          openWeatherAPIKey={key}
          theme="light"
        />
      );
    }
    ```

-   Dark Theme

    ```JSX
      import React from 'react';
      import { UWeatherWidget } from '@bezalel001/unveel-ww';
      const LightTheme =() => {
        const key = 'some key'; // your openweathermap api key

        return (
          <UWeatherWidget
            openWeatherAPIKey={key}
            theme="dark"
          />
        );
    }

    ```

-   Others

    ```JSX
      import React from 'react';
      import { UWeatherWidget } from '@bezalel001/unveel-ww';

      const WeatherWidget =() => {

        const key = 'some key'; // your openweathermap api key

        return (
          <UWeatherWidget
            openWeatherAPIKey={key}
            periodicallyRefreshDataInSeconds={90}
            theme="dark"
          />
        );
    }
    ```

---

### 📝 Props

| Name | Type | Default | Description |
| ---- | ---- | ------- | ----------- |

| `openWeatherAPIKey` | _string_ | Your API key from [OpenWeatherMap](https://openweathermap.org/) |

| `theme` | _string_| `'dark'` |Takes one of two possible values(`'light'` or `'dark'`) | | `periodicallyRefreshDataInSeconds` | _number_ | `30` | Number of seconds that determines when data should be
refreshed in the background

---

#### 🔨 Development

```
git clone https://github.com/bezalel001/unveel-ww.git
npm install
npm run storybook
```

#### 🧪 Test

`npm run test`

#### 🔧 Build

`npm run rollup`

### License

MIT © [bezalel001](https://github.com/bezalel001)
