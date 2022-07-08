# react-debounced-hook

react-debounced-hook provides with a useDebounced hook.

## Installation

Use the package manager [npm](https://nodejs.org/en/) to install react-simple-spoiler.

```terminal
npm install react-debounced-hook --save
```

## Usage

```tsx
import { useDebounced } from 'react-debounced-hook';

const App = () => {
  const [value, setValue] = useState('');
  const [debounced] = useDebounced(value, 200);

  return (
    <>
      <input
        value={value}
        onChange={event => setValue(event.currentTarget.value)}
      />
      <p>Value: {value}</p>
      <p>Debounced value: {debounced}</p>
    </>
  );
};

export default App;
```

## Arguments

**`value: T`**

Value to make debounced

**`wait: number`**

Number in milliseconds to wait

**`options = { leading: false }`**
if set to true then it immediately update value with first call.

###

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)
