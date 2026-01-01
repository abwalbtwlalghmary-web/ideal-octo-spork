# ideal-octo-spork
البرمجة import React from 'react';
import {Keyboard, StyleSheet, Text, TextInput, TouchableWithoutFeedback, View} from 'react-native';

const App: React.FC = () => {
    return (
        <TouchableWithoutFeedback onPress={Keyboard.dismiss}>
            <View style={styles.container}>
                <Text style={styles.title}>Password Input</Text>
                <Text style={styles.description}>Please enter your password:</Text>
                <TextInput
                    style={styles.input}
                    secureTextEntry={true}
                    placeholder="Password"
                    placeholderTextColor="#a2a2a9"
                />
            </View>
        </TouchableWithoutFeedback>
    );
};

export default App;

const styles = StyleSheet.create({
    container: {
        flex: 1,
        justifyContent: 'center',
        alignItems: 'center',
        backgroundColor: '#0d0d0d',
    },
    title: {
        fontSize: 18,
        fontWeight: 'bold',
        color: '#e5e5e7',
        marginBottom: 5,
    },
    description: {
        fontSize: 14,
        color: '#e5e5e7',
        marginBottom: 10,
    },
    input: {
        height: 40,
        borderColor: '#a2a2a9',
        borderWidth: 1,
        borderRadius: 5,
        width: '80%',
        padding: 10,
        color: '#e5e5e7',
    },
});
