# **Gert Valiakhmetov**

## **Contact Info:**

<img src="https://www.kindpng.com/picc/m/49-496199_icons-envelope-computer-mail-message-email-email-icon.png" alt="" width="25" height="25"/>  - valigertt@gmail.com  
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQ5XJ80wv3Bvg7i_kUoyHhiP6drCfUOTPPEYQ&usqp=CAU" alt="" width="25" height="25"/>  - hertas12  
<img src="https://cdn.iconscout.com/icon/free/png-256/discord-1-555369.png" alt="" width="25" height="25"/>  - Gert#2332  
<img src="https://www.pinpng.com/pngs/m/19-198329_github-octocat-vector-png-pluspng-transparent-small-github.png" alt="" width="25" height="25"/> - [GertValiakhmetov](https://github.com/GertValiakhmetov)
 
 ## **Summary**
 
 My initial goal was to get a junior front-end developer position in a good and friendly company. At the moment I am making every effort to make this happen in reality.
 
 
 ## **Skills**
 
 HTML, CSS, SASS, Javascript, React, Redux, Reactstrap, Styled Components, WebStorm

## **Code examples**

    const ItemList = (props) => {

    const {data, onItemSelected, children: renderLabel} = props;

    const items = data.map((item) => {
        const {id} = item;
        const label = renderLabel(item);

        return (
            <li className='list-group-item'
                key={id}
                onClick={() => onItemSelected(id)}>
                {label}
            </li>
        );
    });

    ItemList.defaultProps = {
        onItemSelected: () => {},
    }

    ItemList.propTypes = {
        onItemSelected: PropTypes.func,
        data: PropTypes.arrayOf(PropTypes.object).isRequired,
        children: PropTypes.func.isRequired
    }

    return (
        <ul className='item-list-margin item-list list-group'>
            {items}
        </ul>
      );
    }; 
